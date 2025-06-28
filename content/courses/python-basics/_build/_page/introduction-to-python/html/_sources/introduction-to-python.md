# Introdução ao Python

\:::{toc}
\:depth: 2
\:::

Python é uma linguagem de programação de alto nível, interpretada e de tipagem dinâmica, amplamente utilizada em ciência de dados, desenvolvimento web, automação, inteligência artificial, entre outros.

## Por que aprender Python?

Python é uma das linguagens mais populares do mundo devido à sua:

* Sintaxe simples e legível
* Comunidade ativa e acolhedora
* Grande número de bibliotecas e frameworks
* Aplicações em diversas áreas do conhecimento

\:::{note}
Python é uma linguagem recomendada tanto para iniciantes quanto para profissionais experientes.
\:::

## Instalando o Python

Para começar, é necessário instalar o Python em seu sistema. Você pode baixá-lo em [python.org](https://www.python.org).

Para verificar a versão instalada, utilize:

```bash
python --version
```

## Primeiro código em Python

Vamos começar com o clássico `Hello, world!`.

```python
print("Hello, world!")
```

## Variáveis e Tipos de Dados

Python permite declarar variáveis de forma simples:

```python
nome = "Maria"
idade = 30
altura = 1.65
is_estudante = True
```

Tipos mais comuns:

| Tipo    | Exemplo        |
| ------- | -------------- |
| `int`   | `42`           |
| `float` | `3.14`         |
| `str`   | `"texto"`      |
| `bool`  | `True`/`False` |

## Operações Matemáticas

```python
a = 10
b = 3

print(a + b)  # Soma
print(a - b)  # Subtração
print(a * b)  # Multiplicação
print(a / b)  # Divisão
print(a // b) # Divisão inteira
print(a % b)  # Módulo
print(a ** b) # Potência
```

## Condicionais

```python
idade = 18

if idade >= 18:
    print("Você é maior de idade.")
else:
    print("Você é menor de idade.")
```

## Laços de Repetição

### `for`

```python
for i in range(5):
    print(i)
```

### `while`

```python
contador = 0
while contador < 5:
    print(contador)
    contador += 1
```

## Funções

```python
def saudacao(nome):
    return f"Olá, {nome}!"

print(saudacao("Carlos"))
```

## Listas

```python
frutas = ["maçã", "banana", "laranja"]
print(frutas[0])      # Acessar elemento
frutas.append("uva")  # Adicionar
print(frutas)
```

## Dicionários

```python
aluno = {"nome": "Ana", "idade": 22, "curso": "Python"}
print(aluno["nome"])
```

## Importando Bibliotecas

```python
import math

print(math.sqrt(16))
```

\:::{warning}
Evite usar nomes de variáveis que conflitem com funções internas do Python, como `list`, `str` ou `sum`.
\:::

## Visualizando Gráficos com Matplotlib

```python
import matplotlib.pyplot as plt

x = [1, 2, 3, 4]
y = [2, 4, 6, 8]

plt.plot(x, y)
plt.title("Gráfico simples")
plt.xlabel("x")
plt.ylabel("y")
plt.grid()
plt.show()
```

## Fórmulas com LaTeX

A fórmula da área de um círculo é:

$$
A = \pi r^2
$$

## Exercício

\:::{admonition} Desafio
Escreva um programa que receba o nome e idade de uma pessoa e diga se ela pode ou não tirar carteira de motorista.
\:::

```python
# Sua solução aqui
```

## Conclusão

Neste capítulo, aprendemos:

* Por que usar Python
* Como instalar e rodar programas simples
* Tipos de dados, operadores e estruturas de controle
* Como criar funções e usar listas e dicionários
* Como importar bibliotecas e gerar gráficos simples

\:::{tip}
Você pode expandir esse conteúdo explorando módulos como `pandas`, `numpy` e `scikit-learn`!
\:::
