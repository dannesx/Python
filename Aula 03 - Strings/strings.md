
# ✨ Strings ✨
> `Concatenando`, `Repetindo`, `Indexando` e `Manipulando` Strings

Nesta aula, vamos explorar como trabalhar com strings em Python. Strings são sequências de caracteres usadas para armazenar texto, e Python oferece muitas maneiras de manipulá-las. Vamos aprender sobre concatenação, repetição, indexação, fatiamento e os métodos mais comuns que podem ser usados com strings.

---

## 💡 O que é uma String? 💡

Uma string é uma sequência de caracteres, ou seja, um conjunto de letras, números ou símbolos. Em Python, uma string pode ser definida entre aspas simples (`'...'`) ou aspas duplas (`"..."`).

Exemplo:
```python
nome = "Python"
```

Aqui, a variável `nome` armazena a palavra "Python".


## ⚡ Concatenando Strings ⚡

Concatenar strings significa juntá-las em uma única string. Em Python, usamos o operador `+` para isso.

```python
nome = "Ana"
sobrenome = "Silva"
nome_completo = nome + " " + sobrenome
print(nome_completo)  # Exibe "Ana Silva"
```

O código acima junta as variáveis `nome` e `sobrenome`, separadas por um espaço (`" "`)

## ⚡ Repetição de Strings ⚡

Você pode repetir uma string várias vezes usando o operador `*`.

```python
riso = "ha" * 3
print(riso)  # Exibe "hahaha"
```

O operador `*` repete a string "ha" três vezes

## ⚡ Tamanho de uma String ⚡

Para saber quantos caracteres uma string contém, usamos a função `len()`.

```python
frase = "Python é divertido!"
tamanho = len(frase)
print("O tamanho da frase é: ", tamanho)
```
```
O tamanho da frase é: 19
```
O código vai contar quantos caracteres a frase tem (incluindo espaços)


## ⚡ Indexação em Strings ⚡

Cada caractere em uma string tem uma posição, chamada de índice. Em Python, a contagem começa do zero. Podemos acessar um caractere específico usando colchetes `[]`.

```python
nome = "Python"
print(nome[0])  # Exibe "P"
print(nome[3])  # Exibe "h"
```

`P` está na posição 0 e `h` está na posição 3


## ⚡ Fatiamento de Strings ⚡

O fatiamento permite pegar partes de uma string. Usamos a sintaxe `[início:fim]`, onde `início` é a posição inicial e `fim` é a posição final (não incluída).

```python
nome = "Python"
print(nome[0:3])  # Exibe "Pyt"
```

O código acima vai exibir "Pyt", que são os caracteres nas posições 0, 1 e 2. O caractere na posição 3 não é incluído.

Também podemos usar a notação `[:fim]` para começar do início, ou `[início:]` para pegar até o final.

```python
print(nome[:4])  # Exibe "Pyth"
print(nome[2:])  # Exibe "thon"
```

## ⚡ Usando f-strings ⚡

As f-strings são uma maneira prática de incluir variáveis diretamente dentro de uma string. Para usá-las, basta adicionar a letra `f` antes das aspas e colocar a variável entre chaves `{}`.

```python
nome = "Ana"
idade = 17
print(f"Meu nome é {nome} e eu tenho {idade} anos.")
```
```
Meu nome é Ana e eu tenho 17 anos.
```

As f-strings permitem que variáveis sejam inseridas diretamente na string, tornando o código mais simples e legível.


## ⚡ Métodos Comuns de Strings ⚡

Python tem vários métodos úteis para trabalhar com strings. Aqui estão alguns dos mais comuns:

### 🔹 `upper()`
Transforma todos os caracteres em maiúsculas.

```python
nome = "python"
print(nome.upper())  # Exibe "PYTHON"
```

### 🔹 `lower()`
Transforma todos os caracteres em minúsculas.

```python
nome = "PYTHON"
print(nome.lower())  # Exibe "python"
```

### 🔹 `strip()`
Remove espaços em branco no início e no fim de uma string.

```python
frase = "  Olá, Mundo!  "
print(frase.strip())  # Exibe "Olá, Mundo!"
```

### 🔹 `replace()`
Substitui partes da string por outra.

```python
frase = "Eu amo Python"
nova_frase = frase.replace("Python", "programar")
print(nova_frase)  # Exibe "Eu amo programar"
```

### 🔹 `split()`
Divide uma string em uma lista de palavras, separadas por um espaço ou outro delimitador.

```python
frase = "Eu amo Python"
palavras = frase.split()
print(palavras)  # Exibe ['Eu', 'amo', 'Python']
```

## 📋 Resumo da Aula 📋

- **Concatenação**: Usa-se `+` para juntar strings.
- **Repetição**: Usa-se `*` para repetir strings.
- **Tamanho**: A função `len()` retorna o tamanho de uma string.
- **Indexação**: Acessa um caractere usando o índice da string.
- **Fatiamento**: Extrai partes da string usando `[início:fim]`.
- **f-strings**: Permite incluir variáveis diretamente em uma string usando `{}`.
- **Métodos Comuns**:
  - `upper()`: Converte para maiúsculas.
  - `lower()`: Converte para minúsculas.
  - `strip()`: Remove espaços.
  - `replace()`: Substitui texto.
  - `split()`: Divide uma string em lista.