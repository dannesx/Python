# Introdução aos Algoritmos em Python
> `input`, `print`, `type` e `operadores matemáticos`

Nesta aula, vamos começar do zero, entendendo o que são algoritmos e aprendendo a usar os primeiros comandos em Python. Ao final da aula, você será capaz de criar pequenos programas interativos que realizam cálculos e exibem resultados.

## O que é um Algoritmo?

Um algoritmo é um conjunto de instruções que seguem uma sequência lógica para resolver um problema ou realizar uma tarefa. Ele é como uma receita de bolo: você segue os passos para alcançar um resultado final.

Imagine que você quer fazer um sanduíche. O algoritmo seria:
1. Pegar o pão
2. Colocar o recheio
3. Fechar o sanduiche
4. Comer

No contexto da programação, o algoritmo é um conjunto de passos que o computador segue para realizar uma tarefa específica.

## Introdução ao Python

Python é uma linguagem de programação muito usada por ser simples e prática. Vamos aprender alguns comandos básicos agora!

### 1. Saída de Dados - `print()`

O comando `print()` é usado para mostrar algo na tela

```python
print("Hello World!")
```

Resultado:
```
Hello World!
``` 

Quando você executa esse código, o Python vai imprimir na tela a frase "Hello World!". Isso é útil para exibir mensagem e resultados

### 2. Entrada de Dados - `input()`

O comando `input()` é usado para receber dados do usuário

```python
nome = input("Qual é o seu nome? ")
print("Olá", nome)
```

Resultado:

```
>>> Qual é o seu nome? [Daniel]
Olá Daniel
```

Esse código pergunta o nome do usuário e depois exibe uma saudação personalizada. O comando `input` espera que o usuário digite algo e armazena esse valor na variável `nome`

### 3. Verificar o Tipo - `type()`

O comando `type()` nos ajuda a saber de que tipo de dado estamos manipulando. Em Python, podemos ter diferentes tipos de dados, como números inteiros, texto (strings), e muito mais

```python
idade = input("Quantos anos você tem? ")
print(type(idade))
```

Resultado:
```
>>> Quantos anos você tem? [26]
<class 'str'>
```

O comando `type(idade)` vai mostrar que o dado que o usuário inseriu é do tipo `str` (string, ou texto), mesmo que seja um número. Isso é importante porque às vezes precisamos converter os tipos de dados

### 4. Operadores Matemáticos

Python também é ótimo para fazer cálculos. Aqui estão alguns dos principais operadores matemáticos:

- `+` (adição)
- `-` (subtração)
- `*` (multiplicação)
- `/` (divisão)
- `**` (potenciação)
- `%` (módulo ou resto de divisão)

Exemplo de uso:

```python
numero1 = int(input("Digite o primeiro número: "))
numero2 = int(input("Digite o segundo número: "))

soma = numero1 + numero2
print("A soma é:", soma)
```

Resultado:

```
>>> Digite o primeiro número: [5]
>>> Digite o segundo número: [4]
A soma é: 9
```

Nesse código, usamos `int()` para converter a entrada do usuário (que inicialmente é uma string) em um número inteiro. Depois, realizamos a soma e mostramos o resultado

## Resumo da Aula

- **Algoritmo:** Um conjunto de passos para resolver um problema
- **Comandos:**
  - `print`: Exibe mensagens na tela
  - `input`: Recebe dados do usuário
  - `type`: Mostra o tipo de dado de uma variável
  - Operadores matemáticos: `+`, `-`, `*`, `/`, `**`, `%`