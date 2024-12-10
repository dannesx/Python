---
marp: true
---

# Introdução ao PySimpleGUI - Criação de Interfaces Gráficas Simples com Python 🖥️🐍

### Objetivo da Aula:
Introduzir o **PySimpleGUI**, uma biblioteca Python para criar interfaces gráficas de maneira fácil e intuitiva. Ao final da aula, você será capaz de criar janelas interativas e entender os conceitos básicos de layouts e eventos.

---

## 1. O que é o PySimpleGUI? 🤔
**PySimpleGUI** é uma biblioteca que simplifica a criação de interfaces gráficas (GUIs) em Python. Ela é baseada em outras bibliotecas como Tkinter, PyQt e WxPython, mas com uma sintaxe simplificada.

### Principais vantagens:
- Fácil de aprender e usar.
- Ideal para protótipos e pequenos projetos.
- Suporte a múltiplos "backends" gráficos, como Tkinter e PyQt.

---

## 2. Instalando e Configurando o PySimpleGUI 🛠️

### Instalação:
Se ainda não tiver o PySimpleGUI instalado, use o comando:
```bash
pip install PySimpleGUI
```

### Importando:
Para começar, importe a biblioteca:
```python
import PySimpleGUI as sg
```

---

## 3. Conceitos Básicos do PySimpleGUI 🧱

### Estrutura de um Programa PySimpleGUI:
Um programa PySimpleGUI é composto por:
1. **Layout**: Define os componentes da interface.
2. **Janela (Window)**: Cria a janela com o layout definido.
3. **Eventos**: Captura interações do usuário, como cliques e entradas de texto.

---

```python
import PySimpleGUI as sg

# Definindo o layout
layout = [[sg.Text('Olá, PySimpleGUI!')],
          [sg.Button('Clique Aqui')]]

# Criando a janela
janela = sg.Window('Minha Primeira Janela', layout)

# Loop de eventos
while True:
    evento, valores = janela.read()
    if evento == sg.WINDOW_CLOSED:  # Fecha a janela
        break

janela.close()
```

---

## 4. Elementos do PySimpleGUI 🖋️

### Texto (`sg.Text`)
Exibe textos na interface.
```python
sg.Text('Exemplo de Texto')
```

### Entrada de Dados (`sg.Input`)
Cria um campo para entrada de texto.
```python
sg.Input(default_text='Digite algo aqui...')
```

---

### Botões (`sg.Button`)
Cria botões interativos.
```python
sg.Button('Enviar')
```

### Outros elementos úteis:
- **Checkbox:** `sg.Checkbox('Opção')`
- **ComboBox:** `sg.Combo(['Opção 1', 'Opção 2'])`
- **Slider:** `sg.Slider(range=(0, 100), orientation='h')`

---

## 5. Criando um Formulário Simples 📋

```python
import PySimpleGUI as sg

# Layout
layout = [
    [sg.Text('Nome:'), sg.Input(key='nome')],
    [sg.Text('Idade:'), sg.Input(key='idade')],
    [sg.Button('Enviar'), sg.Button('Cancelar')]
]

# Janela
janela = sg.Window('Formulário', layout)

# Loop de eventos
while True:
    evento, valores = janela.read()
    if evento == sg.WINDOW_CLOSED or evento == 'Cancelar':
        break
    if evento == 'Enviar':
        sg.popup(f"Olá, {valores['nome']}! Você tem {valores['idade']} anos.")

janela.close()
```

---

## 6. Personalizando a Interface 🎨

### Alterando Estilos:
Você pode personalizar as cores e o tema da interface:
```python
sg.theme('DarkBlue')  # Define um tema
```

Para listar todos os temas disponíveis:
```python
print(sg.theme_list())
```

---

## 7. Conclusão e Próximos Passos 🚀

- **Resumo:** Hoje aprendemos a:
  - Criar janelas e layouts no PySimpleGUI.
  - Utilizar elementos como `Text`, `Input` e `Button`.
  - Capturar e processar eventos interativos.

**Desafio:**
Desenvolver um gerador de senhas fortes com PySimpleGUI

