# 💡 O que são Tipos em Go?

**Tipos** em Go definem a natureza dos dados que uma variável pode armazenar e como esses dados devem ser manipulados.

Cada variável em Go tem um **tipo estático** fixo, o que significa que o tipo é definido no momento da compilação e não pode mudar durante a execução do programa.

### Funções dos Tipos:

1.  **Representação de Dados:** Define como o valor é armazenado na memória (ex: um `int` de 32 bits, um `float64` de 64 bits).
2.  **Operações Permitidas:** Define quais operações são válidas (ex: você pode somar dois `int`, mas não pode usar o operador `+` entre um `int` e um `string`).
3.  **Segurança e Consistência:** A tipagem estática (definida na compilação) torna o Go mais seguro, pois muitos erros de lógica são capturados antes do programa rodar.

### Classificação Básica dos Tipos:

| Categoria | Descrição | Exemplos |
| :--- | :--- | :--- |
| **Primitivos/Básicos** | Tipos fundamentais da linguagem. | `bool`, `int`, `float64`, `string` |
| **Compostos** | Estruturas construídas a partir de tipos básicos. | `slice` (fatia), `map` (mapa), `array` (vetor), `struct` (estrutura) |

---

## I. Tipos de Dados Primitivos e Especiais

| Tipo | Descrição | Sintaxe Literal | Exemplo |
| :--- | :--- | :--- | :--- |
| **`string`** | Sequência imutável de bytes (UTF-8). | **Aspas Duplas (`""`)** | `s := "Hello"` |
| **`rune`** | Caractere Unicode único (alias para `int32`). | **Aspas Simples (`''`)** | `r := 'G'` |
| **`int`** | Inteiro com o tamanho nativo do sistema. | N/A | `i := 10` |
| **`float64`** | Ponto flutuante de Dupla Precisão (o padrão idiomático de Go). | N/A | `f := 3.1415` |
| **`map`** | Coleção não ordenada de pares chave-valor. | N/A | `m := map[string]int{...}` |
| **Ponteiro** | Armazena o **endereço de memória** de outra variável. | `*Tipo` | `p := &x` |

---

## II. Operadores e Sintaxe Chave

| Operador | Nome | Função |
| :--- | :--- | :--- |
| **`:=`** | **Declaração Curta** | Declara, infere o tipo e atribui valor a uma **nova** variável em uma única etapa. |
| **`&`** | **Endereço de** | Retorna o endereço de memória de uma variável. |
| **`*`** | **Desreferenciação** | Acessa o **valor** no endereço de memória apontado por um ponteiro. |
| **`<<=`** | **Atribuição de Deslocamento à Esquerda** | Operação bit a bit: `x = x << y` (multiplica por potência de 2). |
| **`_`** | **Identificador Vazio** | Descarta um valor retornado ou um nome importado, **negando o erro de compilação por não uso**. |

---

## III. Funções e Pacotes Essenciais

### A. Funções Nativas (`built-in`)
| Função | Uso |
| :--- | :--- |
| **`len()`** | Retorna o número de bytes em uma string ou o número de elementos em maps/slices/arrays. |

### B. Pacote `fmt` (I/O)
| Função | Descrição | Verbos de `Printf` Importantes |
| :--- | :--- | :--- |
| **`fmt.Scanln`** | Lê entrada do usuário, parando na quebra de linha. | `%v` (Valor Padrão) |
| **`fmt.Printf`** | Imprime saída formatada. | `%c` (Caractere) |
| **`fmt.Println`** | Imprime o valor seguido de quebra de linha. | `%T` (Tipo da variável) |

### C. Pacote `unicode`
| Função | Uso |
| :--- | :--- |
| **`unicode.IsDigit(r rune)`** | Verifica se o caractere (`rune`) é um dígito numérico. |

---

**Uso de Acesso por Índice (`texto[2]`)**:
Ao acessar uma string por índice, o Go retorna o **byte** (valor numérico) daquele caractere. Use **`%c`** no `fmt.Printf` para imprimir o caractere real (`'l'`) em vez do seu código ASCII (`108`).