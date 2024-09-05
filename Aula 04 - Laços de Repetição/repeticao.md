# ✨ Laços de Repetição ✨

> `for`, `while`, `break` e `continue`

Nesta aula, vamos aprender sobre laços de repetição, também chamados de loops. Eles são essenciais quando você quer executar o mesmo conjunto de instruções várias vezes. Vamos explorar os laços `for` e `while`, além dos comandos `break` e `continue`.

## 💡 O que é um Laço de Repetição? 💡

Um laço de repetição permite que o computador execute repetidamente um bloco de código enquanto uma condição for verdadeira. Isso é útil quando queremos repetir uma tarefa várias vezes sem ter que escrever o mesmo código repetidamente.

**Por exemplo:**  
Se você quiser imprimir os números de 1 a 5 na tela, em vez de escrever `print(1)`, `print(2)` e assim por diante, podemos usar um laço de repetição.

## ⚡ O Laço `for` ⚡

O laço `for` é utilizado para percorrer uma sequência (como uma lista, string ou intervalo de números). A cada repetição, ele executa um bloco de código.

### Exemplo básico com números:

```python
for i in range(1, 6):
    print(i)
```

O comando `range(1, 6)` gera os números de 1 a 5 (o último número, 6, não é incluído). O `for` vai percorrer esses números e imprimir cada um.

### Exemplo com uma lista:

```python
nomes = ["Ana", "João", "Maria"]

for nome in nomes:
    print(f"Olá, {nome}!")
```

O laço percorre cada nome na lista `nomes` e imprime uma saudação personalizada para cada um.

## ⚡ O Laço `while` ⚡

O laço `while` repete um bloco de código enquanto uma condição for verdadeira. Assim que a condição se torna falsa, o laço para.

```python
contador = 1

while contador <= 5:
    print(contador)
    contador += 1
```

Enquanto o valor da variável `contador` for menor ou igual a 5, o laço continua rodando. A cada repetição, o valor de `contador` é incrementado em 1.

## ⚡ O Comando `break` ⚡

O comando `break` serve para interromper o laço de repetição antes que ele termine naturalmente. Isso é útil quando queremos parar a repetição após uma determinada condição ser atendida.

```python
for i in range(1, 11):
    if i == 6:
        break
    print(i)
```

O laço imprime os números de 1 a 5. Quando i é igual a 6, o comando break é acionado e o laço é interrompido.

## ⚡ O Comando continue ⚡

O comando `continue` pula a iteração atual do laço e vai diretamente para a próxima. Ou seja, ele interrompe a execução da iteração atual, mas continua com as próximas.

```python
for i in range(1, 6):
    if i == 3:
        continue
    print(i)
```

O número 3 não será impresso. Quando `i` for igual a 3, o comando `continue` vai pular essa iteração e passar diretamente para o próximo número.

## 📋 Resumo da Aula 📋

- **`for`**: Usado para percorrer uma sequência (lista, string, intervalo de números).
- **`while`**: Repete o código enquanto a condição for verdadeira.
- **`break`**: Interrompe o laço antes que ele termine.
- **`continue`**: Pula a iteração atual, mas continua com o laço.
