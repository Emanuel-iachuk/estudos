# Go - Tipos Primitivos 



## 1. Números Inteiros (`int` e Variações)

Os tipos inteiros armazenam números inteiros (positivos e negativos).

| Tipo Padrão | Tamanho | Descrição |
| :--- | :--- | :--- |
| **`int`** | Depende da arquitetura (32 ou 64 bits). | Tipo comum e recomendado para contadores e valores gerais. |
| **`uint`** | Inteiro sem sinal (apenas positivo). | Usado para valores que nunca serão negativos, como tamanhos de coleções. |

### Tipos de Tamanho Fixo:
Para otimização de memória ou interoperabilidade, Go oferece tipos com tamanho explícito:
* **Assinados (Signed):** `int8`, `int16`, `int32`, `int64`
* **Não Assinados (Unsigned):** `uint8` (o famoso **`byte`**), `uint16`, `uint32`, `uint64`

### Verbos de Formatação (`fmt`):
* `%d`: Decimal padrão.
* `%b`: Binário.
* `%x`: Hexadecimal.

**`Exemplo:`**
```GO
package main

import "fmt"

func main() {
    // Declaração do tipo int padrão (dependente da arquitetura)
    contador := 255
    
    // uint8 (byte) é útil para trabalhar com dados de rede e arquivos
    flag := uint8(20) 

    fmt.Println("--- 1. NÚMEROS INTEIROS ---")
    fmt.Printf("Contador: %d (Decimal)\n", contador)
    fmt.Printf("Contador: %b (Binário)\n", contador)
    fmt.Printf("Contador: %x (Hexadecimal)\n", contador)
    
    // Adicionando um int e um uint8. O Go exige conversão explícita:
    soma := contador + int(flag) 
    fmt.Printf("Soma (int + uint8): %d\n", soma)
}
```

---
## 2. Números de Ponto Flutuante (Decimais)

Os tipos de ponto flutuante armazenam números decimais. Eles são essenciais para cálculos que exigem precisão fracionária.

| Tipo | Precisão | Uso |
| :--- | :--- | :--- |
| **`float32`** | Menos preciso (cerca de 6-7 dígitos decimais). | Usado para economizar memória onde a precisão alta não é crucial. |
| **`float64`** | Mais preciso (cerca de 15-16 dígitos decimais). | **O tipo padrão** para a maioria dos cálculos. Se você usar a inferência (`:=`), o Go assumirá `float64`. |

### Constantes e Variáveis
* **Declaração:** `PI := 3.14159` (Go infere `float64`)
* **Constantes Matemáticas:** Go usa `float64` para suas constantes matemáticas, como `math.Pi`.

### Verbos de Formatação (`fmt`):
| Verbo | Descrição | Exemplo de Saída |
| :--- | :--- | :--- |
| **`%f`** | Formato de ponto flutuante fixo. | `3.141593` |
| **`%.2f`** | Ponto flutuante com 2 casas decimais. | `3.14` |
| **`%g`** | Formato geral, usa o mais curto entre `%e` (notação científica) e `%f`. | `3.14159` ou `3.14159e+00` |
| **`%v`** | Valor padrão, mostra a precisão total. | `3.141592653589793` |

**`Exemplo:`**
```Go
package main

import (
	"fmt"
	"math"
)

func main() {
	// float64 inferido automaticamente
	taxaJuros := 0.057891234567 
	
	fmt.Println("\n--- 2. NÚMEROS DE PONTO FLUTUANTE ---")
	
	// %v: Mostra a precisão total do float64
	fmt.Printf("Taxa (Vazamento total - %%v): %v\n", taxaJuros) 
	
	// %.2f: Limita a duas casas decimais (útil para moeda)
	fmt.Printf("Taxa (Formato de Moeda - %%.2f): %.2f\n", taxaJuros) 
	
	// %g: Usa notação científica se o valor for muito grande/pequeno
	fmt.Printf("PI (Formato Geral - %%g): %g\n", math.Pi) 
}
```

---

## 3. Strings e Caracteres

Strings em Go são coleções de bytes **imutáveis** (não podem ser alteradas depois de criadas).

* **Declaração Padrão:** Usa aspas duplas (`"`).
    * Exemplo: `nome := "Emanuel"`
* **Strings Raw (Raw String Literals):** Usam crases (`` ` ``). Preservam quebras de linha e evitam a necessidade de *escape* de caracteres (ótimo para RegEx ou queries SQL).
    * Exemplo: `query := \`SELECT * FROM users\``

### Caracteres (`rune`):
* Um único caractere Unicode é representado pelo tipo **`rune`** (que é um alias para `int32`). Usa aspas simples (`'`).

**`Exemplo:`**
```GO
package main

import "fmt"

func main() {
	// String padrão: O \n é interpretado como quebra de linha (Escape)
	mensagemPadrao := "Olá, Go!\nBem-vindo."
	
	// Raw String: O conteúdo entre ` ` é literal, sem escape.
	// Útil para expressões regulares ou caminhos de arquivo.
	regex := `\s\d{3}\s` 

	// Um rune (caractere Unicode)
	letraA := 'A' 

	fmt.Println("\n--- 3. STRINGS E CARACTERES ---")
	fmt.Println("String Padrão (com escape):")
	fmt.Println(mensagemPadrao)

	fmt.Printf("String Raw (sem escape): %s\n", regex)
	
	// %c: Verbo para caractere/rune
	fmt.Printf("Tipo rune (%T): %c\n", letraA, letraA)
}
```

---

## 4. Booleanos (`bool`)

Armazenam apenas dois valores lógicos, usados em controle de fluxo:

* **`true`**
* **`false`**

### Uso e Formatação:
* **Exemplo:** `usuarioAtivo := true`
* **Verbo de Formatação:** **`%t`** (para booleanos).

**`Exemplo:`**
```GO
package main

import "fmt"

func main() {
	// Declaração e inicialização booleana
	autenticado := true 
	
	fmt.Println("\n--- 4. BOOLEANOS ---")
	
	// %t: Verbo para booleano
	fmt.Printf("Status de autenticação (%%t): %t\n", autenticado) 

	// Uso em controle de fluxo
	if autenticado {
		fmt.Println("Acesso concedido!")
	} else {
		fmt.Println("Acesso negado.")
	}
}
```