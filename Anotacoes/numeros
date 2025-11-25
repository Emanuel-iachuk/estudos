# 🔢 Números em Go

O Go é uma linguagem rigorosa quanto aos tipos numéricos, oferecendo controle total sobre o **tamanho (bits)** e o **sinal** (positivo/negativo) dos dados.

---

## 1. Números Inteiros (`int` e `uint`)

Os inteiros vêm em duas categorias principais:

### Inteiros Assinados (`int*`)

Podem armazenar valores **positivos, zero e negativos**.

| Tipo | Tamanho (Bits) | Faixa de Valores | Alias Comum | Uso |
| :--- | :--- | :--- | :--- | :--- |
| **`int`** | 32 ou 64 | Depende da arquitetura. | N/A | **Padrão** para a maioria das contagens (uso idiomático). |
| **`int8`** | 8 | De -128 a 127 | N/A | Economia de memória ou comunicação de rede. |
| **`int32`** | 32 | Aprox. $\pm 2$ bilhões | **`rune`** | Usado especificamente para representar caracteres Unicode. |

### Inteiros Não Assinados (`uint*`)

Podem armazenar apenas valores **zero ou positivos**.

| Tipo | Tamanho (Bits) | Faixa de Valores | Alias Comum | Uso |
| :--- | :--- | :--- | :--- | :--- |
| **`uint`** | 32 ou 64 | Depende da arquitetura. | N/A | N/A |
| **`uint8`** | 8 | De 0 a 255 | **`byte`** | Usado para manipular dados binários (como *arrays* de bytes). |

---

## 2. Números de Ponto Flutuante (`float`)

Go usa o padrão IEEE-754. O **`float64`** é o tipo preferencial e padrão.

| Tipo | Precisão | Tamanho (Bits) | Precisão Decimal (Aprox.) | Regra Chave |
| :--- | :--- | :--- | :--- | :--- |
| **`float64`** | **Dupla** | 64 | 15 - 17 dígitos | **Padrão por Inferência** (`x := 3.14` resulta em `float64`). |
| **`float32`** | Simples | 32 | 6 - 7 dígitos | Use apenas para otimização extrema de memória. |

### ⚠️ Cuidados com Floats:

* **Comparação:** **Nunca** use o operador `==` (igualdade) para comparar dois `float`s diretamente, devido à imprecisão da representação binária.
* **Recomendação:** Compare a diferença entre eles com um pequeno valor de tolerância (epsilon $\epsilon$).

---

## 3. Números Complexos

| Tipo | Descrição |
| :--- | :--- |
| **`complex128`** | O tipo padrão, composto por dois `float64` (parte real e imaginária). |

---

## IV. Conceitos Relacionados

| Conceito | Aplicação |
| :--- | :--- |
| **`rune`** | Alias de `int32` usado para representar **caracteres** (letras, símbolos) em Go. |
| **`byte`** | Alias de `uint8` usado para representar um **byte de dados**. |
| **`int` (sem tamanho)** | O tipo `int` sem especificação de tamanho é o **mais idiomático** e deve ser usado para a maioria das contagens e iterações. |