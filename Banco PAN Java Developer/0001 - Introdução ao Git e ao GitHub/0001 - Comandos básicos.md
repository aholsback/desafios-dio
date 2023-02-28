# COMANDOS BÁSICOS

## Mudar de pastas (Change direction)

- Windows: **cd**
- Unix: **cd**

### Exemplos

- **cd /** : Leva para a base do diretório C:\

- **cd Windows** : Seguindo do comando anterior, leva para a pasta Windows do diretório C:\

- **cd ..** : Volta uma pasta anterior

## Listar as pastas

- Windows: **dir**
- Unix: **ls**

## Criar pastas/arquivos

- Windows: **mkdir**
- Unix: **mkdir**

### Exemplo

- **mkdir nome da pasta** : Cria uma nova pasta no caminho que você já está no **cmd**.

## Deletar pastas/arquivos

- Windows: **del / rmdir**
- Unix: **rm -rf**

### Exemplo no Windows

- **del nome da pasta** : Estando na pasta anterior a pasta alvo

	- Limpa somente o que está dentro da pasta, mas não exclui a pasta.

- **rmdir nome da pasta /S /Q** : Estando na pasta anterior a pasta alvo

	- Exclui a pasta. Foram usados flags nesse comando para simplificar a exclusão.

### Exemplo no Linux

- **rm -rf nome da pasta/** : Estando na pasta anterior a pasta alvo.

	- Exclui a pasta. Foram usados flags nesse comando para simplificar a exclusão.


- Flag **"rf"**

  - r significa recursivamente, ou seja, todas as subpastas.

  - f significa *"force"*, para não precisar confirmar a exclusão de cada subpasta.


## Limpar a tela

- Windows: **cls**
- Unix: **clear**
- Terminal Bash: **CTRL+L**

## Auto completar

- Windows: Tecla **TAB**
- Unix: Tecla **TAB**

## Criar arquivo de texto pelo terminal

- **echo frase > frase.txt** : Cria um arquivo chamado "frase.txt" contendo a frase "frase" no caminho em que você já está no **cmd**.

	- **echo** : Printa de volta no terminal uma frase, um texto.

## Mover um arquivo

- Terminal Bash

      mv nome do arquivo que será movido caminho da pasta para onde o arquivo será movido

### Exemplo

	mv strogonoff.md ./receitas/

> **strogonoff. md** é o arquivo a ser movido.

> **./receitas/** é a pasta para onde o arquivo será movido.

> **./** significa que eu já estou dentro da pasta anterior a pasta receitas.