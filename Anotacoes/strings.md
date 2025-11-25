# 📄 Strings em Go: Sequências de Bytes e Runes

Em Go, o tipo **`string`** é uma sequência **imutável** de **bytes** codificada em **UTF-8**.

## I. Conceitos Fundamentais

### 1. Imutabilidade
* O conteúdo de uma *string* **não pode ser alterado** após a sua criação.
* Qualquer operação que pareça modificar uma *string* (ex: concatenação, manipulação) na verdade cria uma **nova *string*** na memória.

### 2. A Diferença Crucial: Byte vs. Rune

A chave para entender *strings* em Go é distinguir entre `byte` e `rune`.

| Tipo | Alias de | Propósito | Sintaxe | Tamanho (Bytes) |
| :--- | :--- | :--- | :--- | :--- |
| **`string`** | N/A | Sequência de bytes. | **Aspas Duplas (`"texto"`)** | Variável |
| **`byte`** | `uint8` | Representa **um único byte** de dados. | N/A | 1 (Sempre) |
| **`rune`** | `int32` | Representa um **caractere Unicode** (o ponto de código). | **Aspas Simples (`'c'`)** | 1 a 4 (Variável em UTF-8) |

**Exemplo UTF-8:**
O caractere especial **`á`** (A acentuado) é representado por um único **`rune`**, mas ocupa **dois `bytes`** em uma *string* UTF-8.

---

## II. Acesso e Manipulação

### 1. Comprimento (`len()`)

A função `len()` retorna o **número de bytes** na *string*, e não o número de caracteres (runes).

```go
s := "Olá" // O 'á' é um rune, mas dois bytes.
len(s)     // Retorna 5 (O, l, á-byte1, á-byte2)