# Codigos Uteis

## 1 - [Representação Generica de Objetos em Python](#1---representação-generica-de-objetos-em-python)



### 1 => Representação Generica de Objetos em Python

- Este código utiliza métodos especiais (dunder) para criar uma representação em string que funciona para qualquer objeto, independentemente de seus atributos.

## Exemplo de uso

```python
class Bicicleta:
    def __init__(self, cor, modelo, ano):
        self.cor = cor
        self.modelo = modelo
        self.ano = ano
        
    # Representação de um objeto da classe
    def __str__(self):
        return f"{self.__class__.__name__}: {', '.join(f'{chave} => {valor}' for chave, valor in self.__dict__.items())}"


b1 = Bicicleta("Vermelha", "Caloi", 2020)
print(b1) # Saída: Bicicleta: cor => Vermelha, modelo => Caloi, ano => 2020
```
### Como funciona?

- ``self.__class__.__name__``: Pega o nome da classe (Bicicleta).

- `self.__dict__`: Retorna um dicionário com os atributos do objeto e seus valores.

- `f'{chave} => {valor}'`: Formata cada par chave-valor do dicionário.

- `', '.join(...)`: Junta todos os pares chave-valor em uma única string, separados por vírgulas.