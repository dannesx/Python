
# ✨ Estruturas Condicionais em Python ✨
> `if`, `else`, `elif`, `Operadores Lógicos` e `Booleanos`

Nesta aula, vamos aprender sobre estruturas condicionais em Python. Elas são essenciais para tomar decisões no código, permitindo que diferentes ações sejam executadas dependendo de uma condição. Também vamos aprender como usar operadores lógicos para comparar valores.

---

## 💡 O que são Estruturas Condicionais? 💡

As estruturas condicionais permitem que seu programa tome decisões baseadas em certas condições. Usamos os comandos `if`, `else`, e `elif` para dizer ao computador o que ele deve fazer em diferentes situações.

Por exemplo:  
Imagine que você vai ao cinema e quer saber se pode comprar um ingresso com desconto. Se você tiver menos de 18 anos ou mais de 60 anos, terá desconto. Caso contrário, pagará o valor normal. 

No código, isso seria representado com uma estrutura condicional.

## ⚡ O Comando `if` ⚡

A estrutura `if` é usada para verificar se uma condição é verdadeira. Se for, o código dentro do bloco `if` será executado.

```python
idade = int(input("Qual a sua idade? "))

if idade < 18:
    print("Você tem direito ao desconto!")
```
```
>>> Qual a sua idade? [16]
Você tem direito ao desconto!
```
Se a idade for menor que 18, o programa vai exibir "Você tem direito ao desconto!". Caso contrário, ele não fará nada.

## ⚡ O Comando `else` ⚡

Usamos `else` para executar um bloco de código quando a condição do `if` não é verdadeira.

```python
idade = int(input("Qual a sua idade? "))

if idade < 18:
    print("Você tem direito ao desconto!")
else:
    print("Você não tem direito ao desconto.")
```
```
>>> Qual a sua idade? [20]
Você não tem direito ao desconto.
```

Se a idade for menor que 18, ele mostra a mensagem do `if`. Caso contrário, ele vai para o `else` e exibe "Você não tem direito ao desconto."

## ⚡ O Comando `elif` ⚡

Se você tiver mais de duas condições para verificar, pode usar `elif`. Ele funciona como um "se não, tente isso".

```python
idade = int(input("Qual a sua idade? "))

if idade < 18:
    print("Você tem direito ao desconto!")
elif idade >= 60:
    print("Você tem direito ao desconto para idosos!")
else:
    print("Você não tem direito ao desconto.")
```
```
>>> Qual a sua idade? [62]
Você tem direito ao desconto para idosos!
```

Agora, se a idade for menor que 18 ou maior ou igual a 60, o usuário recebe um desconto. Caso contrário, o `else` é executado.

## 🔹 Operadores Lógicos

Para fazer comparações dentro das estruturas condicionais, usamos operadores lógicos:

- `==`: Igual a
- `!=`: Diferente de
- `>`: Maior que
- `<`: Menor que
- `>=`: Maior ou igual a
- `<=`: Menor ou igual a

Exemplo:

```python
numero = int(input("Digite um número: "))

if numero == 10:
    print("O número é 10!")
elif numero != 10:
    print("O número não é 10.")
```
```
>>> Digite um número: [5]
O número não é 10.
```

Aqui, verificamos se o número é igual a 10 usando `==`. Se não for, o `elif` entra em ação com `!=`, mostrando que o número é diferente de 10.

## 🔹 Operadores Booleanos: `and`, `or`, `not`

Operadores booleanos permitem combinar várias condições em uma só.

### 🔸 `and`
Ambas as condições devem ser verdadeiras para o código ser executado.

```python
idade = int(input("Qual a sua idade? "))
tem_carteirinha = input("Você tem carteirinha de estudante? (s/n) ")

if idade < 18 and tem_carteirinha == 's':
    print("Você tem direito ao desconto com carteirinha!")
```
```
>>> Qual a sua idade? [16]
>>> Você tem carteirinha de estudante? (s/n) [s]
Você tem direito ao desconto com carteirinha!
```

### 🔸 `or`
Uma das condições precisa ser verdadeira para o código ser executado.

```python
idade = int(input("Qual a sua idade? "))

if idade < 18 or idade >= 60:
    print("Você tem direito ao desconto!")
```
```
>>> Qual a sua idade? [70]
Você tem direito ao desconto!
```

### 🔸 `not`
Inverte o valor da condição. Se for `True`, vira `False`, e vice-versa.

```python
desconto = False

if not desconto:
    print("Você não tem desconto.")
```
```
Você não tem desconto.
```

O operador `not` inverte o valor de `desconto`. Como ele era `False`, o `not` faz a condição se tornar verdadeira.

---

## 📋 Resumo da Aula 📋

- **Estruturas Condicionais**:
  - `if`: Verifica se uma condição é verdadeira.
  - `else`: Executa um bloco de código quando o `if` é falso.
  - `elif`: Verifica outras condições se o `if` for falso.
  
- **Operadores Lógicos**:
  - `==`: Igual a
  - `!=`: Diferente de
  - `>` e `<`: Maior que e Menor que
  - `>=` e `<=`: Maior ou igual, Menor ou igual

- **Operadores Booleanos:**
  - `and`: Ambas as condições devem ser verdadeiras.
  - `or`: Apenas uma condição precisa ser verdadeira.
  - `not`: Inverte o valor da condição.
