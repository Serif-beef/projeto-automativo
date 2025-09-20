### Código em Python que utiliza a biblioteca PyAutoGUI para automatizar tarefas usando o os periféricos do computador.

```
import pandas
import pyautogui
from time import sleep

# 1
# abrir o chome
pyautogui.press('win')
pyautogui.write('Chome')
pyautogui.press("enter")
sleep(2)
pyautogui.press("tab")
pyautogui.press("enter")
pyautogui.PAUSE = 2.0
sleep(2)

# digitar site
pyautogui.write("https://dlp.hashtagtreinamentos.com/python/intensivao/login")
pyautogui.press("enter")
sleep(3)
# esperar 3s

# fazer login
pyautogui.press('tab')
sleep(2)

pyautogui.write("nome")

pyautogui.press("tab")
pyautogui.write("senha")
pyautogui.press("enter")


tabela = pandas.read_csv("Nova pasta/produtos.csv")

print(tabela)

# Passo 4: Cadastrar 1 produto

for linha in tabela.index:

    pyautogui.press("tab")

    codigo = tabela.loc[linha, "codigo"]
    pyautogui.write(codigo)

    pyautogui.press("tab")  # passar para o próximo campo
    marca = tabela.loc[linha, "marca"]
    pyautogui.write(marca)

    pyautogui.press("tab")  # passar para o próximo campo
    tipo = tabela.loc[linha, "tipo"]
    pyautogui.write(tipo)

    pyautogui.press("tab")
    categoria = "1"
    pyautogui.write(categoria)

    pyautogui.press("tab")
    preco_unitario = "25.95"
    pyautogui.write(preco_unitario)

    pyautogui.press("tab")
    custo = "6.50"
    pyautogui.write(custo)

    pyautogui.press("tab")
    obs = ""
    pyautogui.write(obs)

    pyautogui.press("tab")
    pyautogui.press("enter")


    pyautogui.scroll(1000)

# Passo 5: Repetir para todos os produtos


# pyautogui.hotkey -> aperta uma combinação de teclas
# pyautogui.click -> clicar em algum lugar
# pyautogui.press -> apertar 1 tecla
# pyautogui.write -> escrever um texto

# Passo 1: Entrar no sistema da empresa - https://dlp.hashtagtreinamentos.com/python/intensivao/
# Passo 2: Fazer login
# Passo 3: Importar a base de dados
# Passo 4: Cadastrar 1 produto
# Passo 5: Repetir para todos os produtosSS

# pyautogui -> fazer automações com python
```
