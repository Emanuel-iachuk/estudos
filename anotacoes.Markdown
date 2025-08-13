### Estudos em Python

##### Tópicos abordados:

### 1 => Tipos de dados

### 2 => Modo interativo

### 3 => Variáveis e Constantes

### 4 => Conversão de tipos

### 5 => Funções de entrada e saída

### 6 => Operadores aritméticos/atribuição

### 7 => Operadores de comparação

### 8 => Operadores lógicos

### 9 => Operadores de identidade

### 10 => Operadores de associação

### 11 => Identação e blocos

### 12 => Estruturas condicionais

### 13 => if aninhado

### 14 => if ternário

### 15 => Estruturas de repetição

### 16 => Manipulando strings com Python

### 17 => Junções e centralização

### 18 => Interpolação de variáveis

### 19 => Formatar strings com f-strings

### 20 => Fatiamento de strings

### 21 => String de múltiplas linhas

### 22 => Listas: Criação e Acesso aos Dados

### 23 => Listas: Fatiamento

### 24 => Listas Aninhadas

### 25 => Metodos da classe list

### 26 => Tuplas

### 27 => Conjuntos


- Python é uma linguagem de programação versátil e amplamente usada em diversas áreas, como desenvolvimento web, ciência de dados, automação e inteligência artificial.
- A sintaxe do Python é clara e fácil de aprender, o que a torna uma excelente escolha para iniciantes e profissionais de tecnologia.
- Python foi criado por *Guido van Rossum* e lançado pela primeira vez em 1991. Ela foi criada com o objetivo de facilitar o desenvolvimento de programas de alto desempenho.

- Python é uma linguagem de *tipagem dinâmica*, o que significa que você não precisa declarar o tipo de uma variável ao criá-la. Isso torna o código mais flexível e fácil de escrever.

- Python suporta múltiplos paradigmas de programação, incluindo *programação orientada a objetos*, *programação funcional* e *programação imperativa*. Isso permite que os desenvolvedores escolham o estilo de programação que melhor se adapta às suas necessidades.

- A comunidade Python é muito ativa e oferece uma vasta gama de bibliotecas e frameworks que facilitam o desenvolvimento de aplicações complexas. Algumas das bibliotecas mais populares incluem:
  - **NumPy**: para computação científica e manipulação de arrays.
  - **Pandas**: para análise de dados e manipulação de tabelas.
  - **Matplotlib**: para visualização de dados.
  - **Django**: um framework web robusto para desenvolvimento de aplicações web.
  - **Flask**: um microframework web leve e flexível.

  ### 1 => Tipos de Dados

- Em Python, os tipos de dados mais comuns incluem:

  - *Inteiros*: `int` => números inteiros, como 1, 2, 3.

  - *Números de ponto flutuante*: `float` => números com casas decimais, como 1.0, 2.5, 3.14.

  - *Booleanos*: `bool` => valores lógicos, como `True` ou `False`.

  - *Strings*: `str` => sequências de caracteres, como "Olá, mundo!".

  - *Listas*: `list` => coleções ordenadas de itens, como [1, 2, 3].

  - *Dicionários*: `dict` => coleções de pares chave-valor, como {"nome": "João", "idade": 30}.

  - *Tuplas*: `tuple` => coleções ordenadas e imutáveis de itens, como (1, 2, 3).

  - *Conjuntos*: `set` => coleções não ordenadas de itens únicos, como {1, 2, 3}.

### 2 => Modo interativo

- O modo interativo do Python permite que você execute comandos e veja os resultados imediatamente. É uma ótima maneira de testar pequenos trechos de código e aprender a linguagem.

- Para iniciar o modo interativo, basta abrir um terminal e digitar `python` ou `python3`, dependendo da sua instalação. Você verá um prompt onde pode digitar comandos Python diretamente.

- No modo interativo, você pode executar expressões e ver os resultados imediatamente. Por exemplo:
  ```python
  >>> 2 + 3
  5
  >>> nome = "Python"
  >>> print(nome)
  Python
  ```

- O modo interativo também permite que você execute scripts externos, como arquivos .py. Para executar um script, basta digitar o comando `python nome_do_script.py`.

- Você pode sair do modo interativo digitando `exit()` ou pressionando `Ctrl + D`.

- O modo interativo é uma ferramenta poderosa para aprender e experimentar com Python, permitindo que você veja os resultados de suas ações imediatamente.

- O modo interativo tambem tem uma função chamada `help()`, que fornece informações sobre funções, módulos e objetos disponíveis no Python. Por exemplo:
  ```python
  >>> help(print)
  ```
- A função `help()` é uma especie de documentação interativa que permite explorar as funcionalidades do Python diretamente no terminal.

### 3 => Variáveis e Constantes

- *Variáveis* devem ser usadas quando um valor pode ou será alterado durante a execução do programa.

- Em Python, *variáveis* são usadas para armazenar dados que podem ser alterados durante a execução do programa. Elas são criadas simplesmente atribuindo um valor a um nome, sem a necessidade de declaração explícita de tipo.

- Em Python, *variáveis* são criadas simplesmente atribuindo um valor a um nome. Por exemplo:
  ```python
  x = 10
  nome = "João"
  ```

- *Constantes* devem ser usadas para armazenar valores que não devem ser alterados exemplos(*CPF, CNPJ, cadastros, etc.*).

- É uma boa prática usar o *snake_case*(*snake_case é um padrão de nomenclatura de variáveis onde as palavras são separadas por tracos baixos ( _ )*) para nomear constantes em Python e a forma mais usada pela comunidade.

- Exemplo de *snake_case*:
  ```python
  numero_de_tentativas = 5
  limite_de_idade = 18
  ```

- *Constantes* em Python são geralmente definidas usando letras maiúsculas. Por exemplo:
  ```python
  PI = 3.14
  NOME = "Maria"
  ```
- Python não possui uma sintaxe específica para declarar *constantes*, mas é uma convenção seguir o uso de letras maiúsculas para indicar que um valor não deve ser alterado.

### 4 => Conversão de Tipos

- Em Python, é comum precisar converter um valor de um tipo para outro. Isso pode ser feito usando funções de conversão integradas, como:
  - `int()`: converte um valor para um inteiro.
  - `float()`: converte um valor para um número de ponto flutuante.
  - `str()`: converte um valor para uma string.

- Exemplos de conversão de tipos:
  ```python
  numero = 10
  texto = str(numero)  # Converte o número para uma string
  ```

### 5 => Funções de Entrada e Saída

- Em Python, é comum precisar ler e escrever dados de entrada e saída. Isso pode ser feito usando funções integradas, como:

  - `input()`: lê uma entrada do usuário e a converte para uma string.

  - `print()`: exibe uma saída no terminal.

  - `int(input())`: lê uma entrada do usuário e a converte diretamente para um inteiro.
  - `float(input())`: lê uma entrada do usuário e a converte diretamente para um número de ponto flutuante.

  - Exemplos de uso das funções de entrada e saída:
    ```python
    nome = input("Digite seu nome: ")
    idade = int(input("Digite sua idade: "))
    print("Ola,", nome, "voce tem", idade, "anos")
    ```

  - `end`: parâmetro da função `print()` que permite especificar o que deve ser impresso no final da saída. Por padrão, é uma nova linha (`\n`), mas pode ser alterado para qualquer string.

  - O parâmetro `end` é útil quando você deseja controlar o que acontece após a impressão de um valor, como evitar a quebra de linha ou adicionar um caractere específico no final da saída.

  - Por exemplo, se você quiser imprimir várias mensagens na mesma linha, pode usar o parâmetro `end` para evitar a quebra de linha automática.

  - Por padrão, o parâmetro `end` é uma nova linha (`\n`), o que significa que cada chamada para `print()` termina com uma quebra de linha. No entanto, você pode personalizar esse comportamento.

  - Exemplo de uso do parâmetro `end`:
    ```python
    print("Olá", end=", ")
    print("mundo!")
    ```
    Saída: `Olá, mundo!`

  - `sep`: parâmetro da função `print()` que permite especificar o separador entre os valores a serem impressos. Por padrão, é um espaço em branco (` `), mas pode ser alterado para qualquer string.

  - O parâmetro `sep` é útil quando você deseja personalizar a forma como os valores são separados na saída.

  - Exemplo de uso do parâmetro `sep`:
    ```python
    print("Olá", "mundo!", sep="-")
    ```
    Saída: `Olá-mundo!`

  - `flush`: parâmetro da função `print()` que permite forçar a saída imediata do buffer, garantindo que a saída seja exibida imediatamente no terminal.

  - O metodo `flush` é útil quando você deseja garantir que a saída seja exibida imediatamente, especialmente em casos onde o buffer pode atrasar a exibição.

  - Por padrão, o parâmetro `flush` é `False`, o que significa que a saída pode ser armazenada em buffer e exibida posteriormente. Quando `flush` é definido como `True`, a saída é forçada a ser exibida imediatamente.

  - Exemplo de uso do parâmetro `flush`:
    ```python
    import time
    print("Carregando...", end="", flush=True)
    time.sleep(2)
    print(" Pronto!")
    ```
    Saída: `Carregando... Pronto!`

  - `file`: parâmetro da função `print()` que permite especificar um arquivo para onde a saída deve ser escrita, em vez de exibi-la no terminal. Por padrão, é `sys.stdout`, que representa a saída padrão do terminal.

  - O parâmetro `file` é útil quando você deseja redirecionar a saída para um arquivo em vez de exibi-la no terminal.
  
  - Exemplo de uso do parâmetro `file`:
    ```python
    with open("saida.txt", "w") as arquivo:
        print("Olá, mundo!", file=arquivo)
    ```
    Isso escreverá "Olá, mundo!" no arquivo `saida.txt` em vez de exibi-lo no terminal.

### 6 => Operadores Aritméticos/Atribuição

- Em Python, os *operadores aritméticos* são usados para realizar operações matemáticas básicas.

- Os *operadores de atribuição* são usados para atribuir valores a variáveis e podem ser combinados com os *operadores aritméticos* para realizar operações e atribuições em uma única expressão.

- Exemplos de *operadores de aritméticos*:

  - `+`: adição
  - `-`: subtração
  - `*`: multiplicação
  - `/`: divisão (retorna um número de ponto flutuante)
  - `//`: divisão inteira (retorna o quociente inteiro)
  - `%`: módulo (retorna o resto da divisão)
  - `**`: exponenciação (eleva um número a uma potência)

- Exemplos de *operadores de atribuição*:

  - `=`: atribuição simples (atribui um valor a uma variável)
  - `+=`: adição e atribuição (incrementa o valor da variável)
  - `-=`: subtração e atribuição (decrementa o valor da variável)
  - `*=`: multiplicação e atribuição (multiplica o valor da variável)
  - `/=`: divisão e atribuição (divide o valor da variável)
  - `//=`: divisão inteira e atribuição (divide o valor da variável e retorna o quociente inteiro)
  - `%=`: módulo e atribuição (divide o valor da variável e retorna o resto da divisão)
  - `**=`: exponenciação e atribuição (eleva o valor da variável a uma potência)
- Exemplos de uso dos *operadores aritméticos/atribuição*:
  ```python
  a = 10 
  b = 5
  c = a + b # retorna 15
  d = a - b # retorna 5
  e = a * b # retorna 50
  f = a / b # retorna 2.0
  g = a // b # retorna 2
  h = a % b # retorna 0
  i = a ** b # retorna 100000
  j = a += b # retorna 15
  k = a -= b # retorna 10
  l = a *= b # retorna 50
  m = a /= b # retorna 10.0
  n = a //= b # retorna 10
  o = a %= b # retorna 0
  p = a **= b # retorna 100000
  ```

### 7 => Operadores de Comparação

- Em Python, os *operadores de comparação* são usados para comparar valores e retornar um valor booleano (`True` ou `False`). Os principais *operadores de comparação* incluem:

  - `==`: igual
  - `!=`: diferente
  - `<`: menor que
  - `<=`: menor ou igual a
  - `>`: maior que
  - `>=`: maior ou igual a
- Exemplos de uso dos *operadores de comparação*:
  ```python
  a = 10
  b = 5
  c = a == b #returna False porque 10 não é igual a 5
  d = a != b #returna True porque 10 é diferente de 5
  e = a < b #returna False porque 10 não é menor que 5
  f = a <= b #returna False porque 10 não é menor ou igual a 5
  g = a > b #returna True porque 10 é maior que 5
  h = a >= b #returna True porque 10 é maior ou igual a 5
  ```

### 8 => Operadores Lógicos

- Em Python, os *operadores lógicos* são usados para combinar expressões booleanas e retornar um valor booleano (`True` ou `False`). Os principais *operadores lógicos* incluem:

  - `and`: retorna `True` se ambas as expressões forem verdadeiras
  - `or`: retorna `True` se pelo menos uma das expressões for verdadeira
  - `not`: inverte o valor da expressão (retorna `True` se a expressão for falsa e vice-versa)

- Exemplos de uso dos *operadores lógicos*:
  ```python
  a = 10
  b = 5
  c = a > b and b > 0 #returna True porque ambas as expressões são verdadeiras
  d = a > b or b < 0 #returna True porque pelo menos uma das expressões é verdadeira
  e = not (a > b) #returna False porque a > b é True
  ```

### 9 => Operadores de Identidade
- Em Python, os *operadores de identidade* são usados para verificar se dois objetos são ocupam a mesma posição na memória. Os principais *operadores de identidade* incluem:

  - `is`: retorna `True` se os objetos forem idênticos (ocuparem a mesma posição na memória)

  - `is not`: retorna `True` se os objetos não forem idênticos

- Os *operadores de identidade* são úteis para verificar se duas variáveis referenciam o mesmo objeto, especialmente quando se trabalha com listas, dicionários e outros objetos mutáveis.

- Exemplos de uso dos *operadores de identidade*:
  ```python
  a = [1, 2, 3]
  b = a
  c = a[:]
  d = a is b #returna True porque b é uma referência ao mesmo objeto que a
  e = a is c #returna False porque c é uma cópia de a
  f = a == c #returna True porque os valores de a e c são iguais
  g = a is not c #returna True porque c é uma cópia de a
  h = a is not b #returna False porque b é uma referência ao mesmo objeto que a
  ```

### 10 => Operadores de associação
- Em Python, os *operadores de associação* são usados para verificar se um valor está presente em uma sequência, como listas, tuplas ou strings. Os principais *operadores de associação* incluem:

  - `in`: retorna `True` se o valor estiver presente na sequência
  - `not in`: retorna `True` se o valor não estiver presente na sequência

- Exemplos de uso dos *operadores de associação*:
  ```python
  a = [1, 2, 3]
  b = 2
  c = 4
  d = b in a #returna True porque 2 está presente na lista a
  e = c not in a #returna True porque 4 não está presente na lista a
  ```

### 11 => Identação e blocos

- Em Python, a *indentação* é usada para definir blocos de código. Isso significa que o nível de *indentação* determina quais linhas pertencem a um determinado bloco, como loops, condicionais e funções.

- A *indentação* é obrigatória em Python e deve ser consistente em todo o código. Por padrão, usa-se 4 espaços para cada nível de *indentação*, mas você pode usar tabulações se preferir, desde que seja consistente.

- Exemplos de uso da *indentação*:
  ```python
  if True:
      print("Isso está dentro do bloco if")
      if False:
          print("Isso está dentro do bloco if aninhado")
  print("Isso está fora do bloco if")
  ```

### 12 => Estruturas Condicionais
- Em Python, as *estruturas condicionais* são usadas para executar diferentes blocos de código com base em condições. As principais *estruturas condicionais* incluem:

  - `if`: executa um bloco de código se a condição for verdadeira
  - `elif`: (abreviação de "else if") executa um bloco de código se a condição anterior for falsa e esta condição for verdadeira
  - `else`: executa um bloco de código se todas as condições anteriores forem falsas

- Exemplos de uso das *estruturas condicionais*:
  ```python
  if True:
      print("A condição é verdadeira")
  elif False:
      print("A condição é falsa, mas esta é verdadeira")
  else:
      print("Todas as condições anteriores são falsas")
  ```
- As *estruturas condicionais* são úteis para controlar o fluxo do programa e tomar decisões com base em condições específicas.

- As *estruturas condicionais* também podem ser aninhadas, ou seja, você pode ter uma *estrutura condicional* dentro de outra. Isso permite criar lógica mais complexa e tomar decisões com base em múltiplas condições.

### 13 => if aninhado:

- Em Python, você pode aninhar *estruturas condicionais* para criar lógica mais complexa. Isso significa que você pode ter uma *estrutura condicional* dentro de outra.

- O uso de *if aninhado* permite que você verifique condições adicionais dentro de um bloco de código já existente, o que pode ser útil para tomar decisões mais específicas.

- Exemplo de uso de *if aninhado*:
  ```python
  idade = 20
  if idade >= 18:
      print("Você é maior de idade")
      if idade >= 65:
          print("Você é um idoso")
      else:
          print("Você ainda é jovem")
  else:
      print("Você é menor de idade")
  ```
- No exemplo acima, a primeira *estrutura condicional* verifica se a idade é maior ou igual a 18. Se for, ela imprime uma mensagem e verifica se a idade é maior ou igual a 65, imprimindo uma mensagem adicional dependendo do resultado.

- A segunda *estrutura condicional* verifica se a idade é menor que 18, imprimindo uma mensagem correspondente.

### 14 => if ternario:

- Em Python, você pode usar uma expressão condicional (também conhecida como *if ternário*) para atribuir um valor a uma variável com base em uma condição. A sintaxe é a seguinte:

  ```python
  variavel = valor_se_verdadeiro if condicao else valor_se_falso
  ```

  - o *if ternário* é usado quando fazer algo mais simples e conciso do que usar uma *estrutura condicional* completa.

  - Ele permite que você atribua um valor a uma variável com base em uma condição, tornando o código mais legível e compacto.

- Exemplo de uso de *if ternário*:
  ```python
  idade = 20
  status = "Maior de idade" if idade >= 18 else "Menor de idade"
  print(status)
  ```
  - Caso a condição `idade >= 18` seja verdadeira, a variável `status` receberá o valor `"Maior de idade"`. Caso contrário, receberá o valor `"Menor de idade"`.

### 15 => Estruturas de repetição

- Em Python, as *estruturas de repetição* são usadas para executar um bloco de código várias vezes com base em uma condição ou em uma sequência de elementos. As principais *estruturas de repetição* incluem:

  - `for`: itera sobre uma sequência (como listas, tuplas ou strings) e executa um bloco de código para cada elemento

  - `while`: executa um bloco de código enquanto uma condição for verdadeira

- As *estruturas de repetição* são úteis para executar tarefas repetitivas, como percorrer listas, realizar cálculos ou processar dados.

Exemplos de uso das *estruturas de repetição*:
- Com o `for`:
  ```python
  for i in range(5):
      print("Iteração", i)
  ```
- Com o `while`:
  ```python
  i = 0
  while i < 5:
      print("Iteração", i)
      i += 1
  ```

- As *estruturas de repetição* podem ser usadas para criar lógica mais complexa e tornar o código mais eficiente e eficaz.


### 16 => Manipulando strings com Python
- Em Python, as strings são sequências de caracteres e podem ser manipuladas de várias maneiras. Algumas das operações mais comuns incluem:

  - *Maiúsculas*: converter uma string para letras maiúsculas usando o método `.upper()`.
  exemplo:
  ```python
  nome = "joão"
  nome_maiusculo = nome.upper()
  print(nome_maiusculo)  # Saída: JOÃO
  ```

  - *Minúsculas*: converter uma string para letras minúsculas usando o método `.lower()`.
  exemplo:
  ```python
  nome = "JOÃO"
  nome_minusculo = nome.lower()
  print(nome_minusculo)  # Saída: joão
  ```

  - *Título*: converter a primeira letra de cada palavra para maiúscula usando o método `.title()`.
  exemplo:
  ```python
  nome = "joão da silva"
  nome_titulo = nome.title()
  print(nome_titulo)  # Saída: João Da Silva
  ```

  - *Eliminação de espaços em branco*: remover espaços em branco no início e no final de uma string usando o método `.strip()`.
  exemplo:
  ```python
  nome = "   joão   "
  nome_sem_espacos = nome.strip()
  print(nome_sem_espacos)  # Saída: "joão"
  ```
  - `lstrip()` remove os espaços do início da string.
  exemplo:
  ```python
  nome = "   joão   "
  nome_sem_espacos = nome.lstrip()
  print(nome_sem_espacos)  # Saída: "joão   "
  ```
  - `rstrip()` remove os espaços do final da string.
  exemplo:
  ```python
  nome = "   joão   "
  nome_sem_espacos = nome.rstrip()
  print(nome_sem_espacos)  # Saída: "   joão"
  ```

### 17 => Junções e centralização

- Podemos usar o metodo `center()` para centralizar uma string em um determinado tamanho.
  exemplo:
  ```python
  nome = "joão"
  nome_centralizado = nome.center(10, "#")
  print(nome_centralizado)  # Saída: "###joão###"
  ```
- O método `center()` recebe dois argumentos: o tamanho total da string resultante e o caractere de preenchimento (opcional) que será usado para preencher os espaços restantes.

- Podemos usar o metodo `join()` para unir uma lista de strings em uma única string, usando um separador específico.
  exemplo:
  ```python
  nomes = ["joão", "maria", "pedro"]
  nomes_unidos = ", ".join(nomes)
  print(nomes_unidos)  # Saída: "joão, maria, pedro"
  ```
- O método `join()` recebe um iterável (como uma lista ou tupla) e retorna uma string resultante da concatenação dos elementos, separados pelo separador especificado.

- Também podemos usar o metodo `join()` para separe strings com um caractere específico.
  exemplo:
  ```python
  numeros = ["1", "2", "3"]
  numeros_unidos = "-".join(numeros)
  print(numeros_unidos)  # Saída: "1-2-3"
  ```

### 18 => Interpolação de variáveis

- Em Python, podemos usar o operador de interpolação de variáveis para incluir o valor de uma variável dentro de uma string usando o formato de string f.
  exemplo:
  ```python
  nome = "joão"
  idade = 25
  mensagem = f"Olá, meu nome é {nome} e eu tenho {idade} anos."
  print(mensagem)
  ```
- A interpolação de variáveis permite que você crie strings dinâmicas, onde o valor das variáveis é inserido diretamente na string, tornando o código mais legível e fácil de entender.

### 19 => Formatar strings com f-strings

- Utilizamos o *:.2f* para formatar números de ponto flutuante com duas casas decimais.
  exemplo:
  ```python
  preco = 19.9999
  mensagem = f"O preço do produto é R${preco:.2f}."
  print(mensagem)  # Saída: "O preço do produto é R$19.99."
  ```
- Tambem podemos usar o *:10.2f* para formatar números de ponto flutuante com 10 casas decimais.
  exemplo:
  ```python
  preco = 19.9999
  mensagem = f"O preço do produto é R${preco:10.2f}."
  print(mensagem)  # Saída: "O preço do produto é R$    19.99."
  # O número é alinhado à direita com espaços à esquerda para completar 10 caracteres.
  ```
- As *f-strings* são uma maneira eficiente e legível de formatar strings em Python, permitindo a inclusão de expressões diretamente dentro das chaves `{}`.

### 20 => Fatiamento de strings
- Em Python, podemos usar o fatiamento de strings para extrair partes específicas de uma string. O fatiamento é feito usando a notação `string[inicio:fim:passo]`, onde:

  - `inicio`: índice inicial (inclusivo)
  - `fim`: índice final (exclusivo)
  - `passo`: intervalo entre os índices (opcional)
- Exemplo de fatiamento de strings:
  ```python
  texto = "Olá, mundo!"
  print(texto[0:5])  # Saída: "Olá, "
  print(texto[7:])   # Saída: "mundo!"
  print(texto[:5])   # Saída: "Olá, "
  print(texto[::2])  # Saída: "O,mn!"
  print(texto[::-1]) # Saída: "!odnum ,álO"
  ```

- O fatiamento de strings é uma ferramenta poderosa que permite acessar e manipular partes específicas de uma string de forma eficiente.

### 21 => String de múltiplas linhas

- Em Python, podemos criar strings de múltiplas linhas usando aspas triplas (`"""` ou `'''`). Isso permite que você escreva uma string que abrange várias linhas sem precisar usar caracteres de escape para novas linhas.

- Exemplo de string de múltiplas linhas:
  ```python
  mensagem = """Esta é uma string
  que abrange várias linhas.
  Você pode escrever texto aqui
  sem se preocupar com quebras de linha."""
  print(mensagem)
  ```

- As strings de múltiplas linhas são úteis para armazenar textos longos, como descrições, mensagens ou até mesmo blocos de código, sem a necessidade de concatenar várias strings.

### 22 => Listas: Criação e Acesso aos Dados

- Em Python, as listas são coleções ordenadas de elementos que podem conter diferentes tipos de dados. Elas são criadas usando colchetes `[]` e os elementos são separados por vírgulas.
  exemplo:  
  ```python
  numeros = [1, 2, 3, 4, 5]

  letras = ['a', 'b', 'c', 'd']
  misto = [1, 'dois', 3.0, True]
  ```

- As listas em python são mutáveis, Você não precisa declarar o tipo de dados que a lista irá conter, pois Python é uma linguagem de tipagem dinâmica.

- Você tam bem pode criar uma lista usando a palavra-chave `list()`, que converte outros iteráveis em uma lista.
  exemplo:
  ```python
  numeros = list(range(1, 6))  # Cria uma lista de números de 1 a 5
  ```

- Para acessar os elementos de uma lista, você pode usar índices, que começam em 0. Por exemplo, `numeros[0]` acessa o primeiro elemento da lista `numeros`.
- Exemplo de acesso aos dados de uma lista:
  ```python
  numeros = [1, 2, 3, 4, 5]
  print(numeros[0])  # Saída: 1
  print(numeros[2])  # Saída: 3
  print(numeros[4])  # Saída: 5
  ```
- Para acessar um elemento de uma lista o indice sempre começa em 0, ou seja, o primeiro elemento tem o índice 0, o segundo elemento tem o índice 1, e assim por diante. 

- Você também pode acessar elementos negativos, que contam a partir do final da lista. Por exemplo, `numeros[-1]` acessa o último elemento da lista.
- Exemplo de acesso a elementos negativos:
  ```python
  numeros = [1, 2, 3, 4, 5]
  print(numeros[-1])  # Saída: 5
  print(numeros[-3])  # Saída: 3
  ```

### 23 => Listas: Fatiamento

- As listas também suportam fatiamento, permitindo que você acesse uma sublista de elementos. Por exemplo, `numeros[1:4]` retorna os elementos do índice 1 ao 3 (exclusivo).
- Exemplo de fatiamento de listas:
  ```python
  numeros = [1, 2, 3, 4, 5]
  print(numeros[1:4])  # Saída: [2, 3, 4]
  print(numeros[:3])   # Saída: [1, 2, 3]
  print(numeros[2:])   # Saída: [3, 4, 5]
  print(numeros[::2])  # Saída: [1, 3, 5] (passo de 2)
  ```

 ### 24 => Listas Aninhadas

- Em Python, você pode criar listas aninhadas, que são listas dentro de outras listas. Isso permite organizar dados de forma hierárquica ou multidimensional também chamada de matrizes.

- Exemplo de listas aninhadas:
  ```python
  matriz = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
  print(matriz[0])  # Saída: [1, 2, 3]
  print(matriz[1][2])  # Saída: 6 (acessa o elemento na segunda linha e terceira coluna)
  print(matriz[2][0])  # Saída: 7 (acessa o elemento na terceira linha e primeira coluna)
  print(matriz[-1])    # Saída: [7, 8, 9] (acessa a última linha)
  print(matriz[-1][-1])  # Saída: 9 (acessa o último elemento da última linha)
  ```

- Você pode acessar os elementos de uma lista aninhada usando o metodo *for*:
  ```python
  matriz = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]  
  for linha in matriz:
    for elemento in linha:
      print(elemento)#  a saída seria 1, 2, 3, 4, 5, 6, 7, 8, 9
  ```

### 25 => Metodos da classe list

- *append()*: Adiciona um elemento ao final da lista.
exemplo:
  ```python
  numeros = [1, 2, 3]
  numeros.append(4)  # Adiciona o elemento 4 ao final da lista
  print(numeros)  # Saída: [1, 2, 3, 4]
  ```

- *copy():* Cria uma cópia da lista.
exemplo:
  ```python
  numeros = [1, 2, 3]
  numeros_copia = numeros.copy()
  print(numeros_copia)  # Saída: [1, 2, 3]
  ```

- *count()*: Conta o número de vezes que um elemento aparece na lista.
exemplo:
  ```python
  numeros = [1, 2, 3, 2, 4, 2]
  print(numeros.count(2))  # Saída: 3
  ```

- *extend()*: Extende a lista adicionando os elementos de outra lista util quando vocé quer adicionar mais de um elemento a uma lista.
exemplo:
  ```python
  numeros = [1, 2, 3]
  outros_numeros = [4, 5, 6]
  numeros.extend(outros_numeros)
  print(numeros)  # Saída: [1, 2, 3, 4, 5, 6]
  ```

- *index()*: Retorna a posição do elemento que você quer encontrar na lista.
exemplo:
  ```python
  numeros = [1, 2, 3, 4, 5]
  print(numeros.index(3))  # Saída: 2
  ```

- *Pop()*: Remove o ultimo elemento da lista ou se desejar tam bem pode remover um elemento especifico da lista.
exemplo:
  ```python
  numeros = [1, 2, 3, 4, 5]
  numeros.pop()  # Remove o ultimo elemento da lista
  print(numeros)  # Saída: [1, 2, 3, 4]
  numeros.pop(1)  # Remove o elemento na posicao 1 da lista
  print(numeros)  # Saída: [1, 3, 4]
  ```

- *remove()*: Remove o primeiro elemento da lista que seja igual ao elemento que vocé quer remover ou seja você escolhe o elemento que vocé quer remover.
exemplo:
  ```python
  numeros = [1, 2, 3, 4, 5]
  numeros.remove(3)  # Remove o elemento 3 da lista
  print(numeros)  # Saída: [1, 2, 4, 5]
  ```

- *reverse()*: Inverte a ordem dos elementos na lista.
exemplo:
  ```python
  numeros = [1, 2, 3, 4, 5]
  numeros.reverse()  # Inverte a ordem dos elementos na lista
  print(numeros)  # Saída: [5, 4, 3, 2, 1]
  ```

- *sort()*: Ordena a lista em ordem alfabetica/crescente.
exemplo:
  ```python
  numeros = [4, 3, 2, 1, 5]
  numeros.sort()  # Ordena a lista em ordem crescente
  print(numeros)  # Saída: [1, 2, 3, 4, 5]
  ```

- Dentro do metodo *sort()* exite os seguintes parâmetros:
  - *reverse = True*: Inverte a ordem dos elementos na lista.
  - *key = str.lower*: Ordena a lista em ordem alfabetica, ignorando maiúsculas e minúsculas.
  - *key = len*: Ordena a lista em ordem crescente de tamanho dos elementos.
  - *key = lambda x: len(x)*: Ordena a lista em ordem crescente de tamanho dos elementos.
  - *key = lambda x: len(x) * -1*: Ordena a lista em ordem decrescente de tamanho dos elementos.
  - Tambem e posivel juntar os parâmetros:
    ```python
    numeros.sort(reverse=True, key=lambda x: len(x)) # Ordena a lista em ordem decrescente de tamanho dos elementos
    ```

- *len()*: Retorna o número de elementos na lista.
exemplo:
  ```python
  numeros = [1, 2, 3, 4, 5]
  print(len(numeros))  # Saída: 5
  ```

- *sorted()*: Retorna uma nova lista com os elementos da lista original ordenados.
exemplo:
  ```python
  numeros = [4, 3, 2, 1, 5]
  numeros_ordenados = sorted(numeros)
  print(numeros_ordenados)  # Saída: [1, 2, 3, 4, 5]
  ```

- No `sorted()` tam existe o `Key()` e `reverse()` e eles fazem a mesma coisa que no `sort()`.

### 26 => Tuplas

- As `tuplas` em Python são listas imutáveis, ou seja, eles podem ser usadas para armazenar valores, mas não podem ser alterados são muito semelhantes as listas
e podem ser usada a palavra reservada `tuple` para cria uma tupla ou pode tam bem usar valores separados por `virgula` detro de parenteses.

- Exemplo de tupla:
  ```python
  numeros = tupla([1, 2, 3, 4, 5])
  print(tupla)  # Saída: (1, 2, 3, 4, 5)
  ```
- Exemplo de tupla com valores separados por virgula:
  ```python
  numeros = (1, 2, 3, 4, 5,)
  print(tupla)  # Saída: (1, 2, 3, 4, 5)
  ```

- Para acessar os elementos de uma tupla, é igual a listas assim podemos usar o `fatiamento` para pegar os valores.

- Exemplo:
  ```python
  numeros = (1, 2, 3, 4, 5,)
  numeros[0]  # Saída: 1
  numeros[2]  # Saída: 3
  numeros[-1]  # Saída: 5
  numeros[1:4]  # Saída: (2, 3, 4)
  ```

- `Tupla alinhadas`: É possivel criar tuplas alinhadas, ou seja, tuplas dentro de tuplas.

- Exemplo:
  ```python
  numeros = ((1, 2, 3), (4, 5, 6), (7, 8, 9))
  print(numeros)  # Saída: ((1, 2, 3), (4, 5, 6), (7, 8, 9))
  print(numeros[0])  # Saída: (1, 2, 3)
  print(numeros[1][2])  # Saída: 6
  print(numeros[2][1])  # Saída: 8
  print(numeros[0][0])  # Saída: 1
  print(numeros[-1][-1])  # Saída: 9
  print(numeros[-1])  # Saída: (7, 8, 9)
  ```

- Tambem e possivel usar o enumerate() para percorrer uma tupla:
  ```python
  numeros = (1, 2, 3, 4, 5)
  for i, numero in enumerate(numeros):
      print(i, numero)# Saída: 0 1
                        #        1 2
                        #        2 3
                        #        3 4
                        #        4 5
  ```

- `Metodos da tupla`:

- `count()`: Conta o número de vezes que um elemento aparece na tupla.
exemplo:
  ```python
  numeros = (1, 2, 3, 2, 4, 2)
  print(numeros.count(2))  # Saída: 3
  ```

- `index()`: Retorna a posição do elemento que você quer encontrar na tupla.
- exemplo:
  ```python
  numeros = (1, 2, 3, 4, 5)
  print(numeros.index(3))  # Saída: 2
  ```

- `len()`: Retorna o número de elementos na tupla.
- exemplo:
  ```python
  numeros = (1, 2, 3, 4, 5)
  print(len(numeros))  # Saída: 5
  ```

### 27 => Conjuntos

- Os `Conjuntos` em Python são listas sem ordem, ou seja, eles podem ser usados para armazenar valores, mas nao podem ser alterados mais eles não podem ter elementos duplicados se em sua lista existem elementos duplicados os conjuntos irao remover os elementos duplicados para dizer que é uma conjunto usamos a palavra reservada `set`.

- Exemplo de conjunto:
  ```python
  numeros = [1, 2, 3, 4, 5, 3, 2, 1]
  conjunto = set(numeros)
  print(conjunto)  # Saída: {1, 2, 3, 4, 5}

  fruta = "banana"
  conjunto = set(fruta)
  print(conjunto)  # Saída: {'a', 'b', 'n'}
  ```

- Tambem e possivel usar o metodo `for` para percorrer um conjunto:
  ```python
  conjunto = {1, 2, 3, 4, 5}
  for numero in conjunto:
      print(numero)  # Saída: 1
                     #        2
                     #        3
                     #        4 
                     #        5
  ```

- A funcão `enumerate()` também pode ser usada para percorrer um conjunto:
  ```python
  conjunto = {"A", "B", "C", "D", "E"}
  for i, numero in enumerate(conjunto):
      print(i, numero)  # Saída: 0 A
                        #        1 B
                        #        2 C
                        #        3 D
                        #        4 E
  ``` 

- Principais metodos do conjunto:

  - `union()`: Une dois conjuntos.
  - exemplo:
    ```python
    conjunto1 = {1, 2, 3}
    conjunto2 = {4, 5, 6}
    conjunto_uniao = conjunto1.union(conjunto2)
    print(conjunto_uniao)  # Saída: {1, 2, 3, 4, 5, 6}
    ```

  - `intersection()`: Retorna os elementos que estao presentes em ambos os conjuntos.
  - exemplo:
    ```python
    conjunto1 = {1, 2, 3}
    conjunto2 = {3, 4, 5}
    conjunto_intersecao = conjunto1.intersection(conjunto2)
    print(conjunto_intersecao)  # Saída: {3}
    ```
  
  - `difference()`: Retorna os elementos que estao presentes no primeiro conjunto, mas nao estao presentes no segundo conjunto.
  - exemplo:
    ```python
    conjunto1 = {1, 2, 3}
    conjunto2 = {3, 4, 5}
    conjunto_diferenca = conjunto1.difference(conjunto2)
    print(conjunto_diferenca)  # Saída: {1, 2}
    ```
  
  - `symmetric_difference()`: Retorna os elementos que estao presentes nos dois conjuntos, menos os elementos que estao presentes em ambos os conjuntos.
  - exemplo:
    ```python
    conjunto1 = {1, 2, 3}
    conjunto2 = {3, 4, 5}
    conjunto_diferenca_simetrica = conjunto1.symmetric_difference(conjunto2)
    print(conjunto_diferenca_simetrica)  # Saída: {1, 2, 4, 5}
    ```
  
  - `issubset()`: Retorna `True` se todos os elementos do primeiro conjunto estao presentes no segundo conjunto.
  - exemplo:
    ```python
    conjunto1 = {1, 2, 3}
    conjunto2 = {1, 2, 3, 4, 5}
    print(conjunto1.issubset(conjunto2))  # Saída: True
    ```
  
  - `issuperset()`: Retorna `True` se todos os elementos do segundo conjunto estao presentes no primeiro conjunto.
  - exemplo:
    ```python
    conjunto1 = {1, 2, 3}
    conjunto2 = {1, 2, 3, 4, 5}
    print(conjunto2.issuperset(conjunto1))  # Saída: True
    ```

  - `isdisjoint()`: Retorna `True` se nenhum dos elementos do primeiro conjunto estao presentes no segundo conjunto.
  - exemplo:
    ```python
    conjunto1 = {1, 2, 3}
    conjunto2 = {4, 5, 6}
    conjunto3 = {1, 2, 3, 4, 5, 6}
    print(conjunto1.isdisjoint(conjunto2))  # Saída: True
    print(conjunto1.isdisjoint(conjunto3))  # Saída: False
    ```

  - `add()`: Adiciona um elemento ao conjunto caso esse elemento esteja presente no conjunto ele sera ignorado.
  - exemplo:
    ```python
    conjunto = {1, 2, 3}
    conjunto.add(4)
    conjunto.add(2) # Elemento iguinorado por ser duplicado
    print(conjunto)  # Saída: {1, 2, 3, 4}
    ```

  - `clear()`: Remove todos os elementos do conjunto.
  - exemplo:
    ```python
    conjunto = {1, 2, 3}
    conjunto.clear()
    print(conjunto)  # Saída: set()
    ```
  
  - `copy()`: Cria uma cópia do conjunto.
  - exemplo:
    ```python
    conjunto = {1, 2, 3}
    conjunto_copia = conjunto.copy()
    print(conjunto_copia)  # Saída: {1, 2, 3}
    ```

  - `discard()`: Remove um elemento do conjunto caso ele esteja presente no conjunto.
  - exemplo:
    ```python
    conjunto = {1, 2, 3}
    conjunto.discard(2)
    print(conjunto)  # Saída: {1, 3}
    ```
  
  - `pop()`: Remove o ultimo elemento do conjunto e o retorna.
  - exemplo:
    ```python
    conjunto = {1, 2, 3}
    elemento_removido = conjunto.pop()
    print(elemento_removido)  # Saída: 3
    print(conjunto)  # Saída: {1, 2}
    ```
  
  