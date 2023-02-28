# PRIMEIROS COMANDOS COM GIT

## Iniciar o repositório do Git

Cria uma pasta oculta onde o Git é iniciado.

	git init

### Exemplo

- Pelo **Git Bash**, entre na pasta que você deseja que seja iniciado o repositório do git;

- Dê o comando;

		git init

- Uma mensagem retornará dizendo que um repositório vazio foi iniciado dentro da pasta que você estava;

- O repositório git será iniciado em uma pasta oculta.

		./ ../ .git/

### Comandos extras

- Para visualizar essa pasta oculta, deve-se digitar o seguinte comando com a *flag* "-a";

		ls -a

- Para entrar dentro da pasta oculta;

		cd .git/

- Para listar os itens dentro dessa pasta oculta;

		ls

- Voltar para a pasta anterior.

		cd ..

## Configuração do Git

Para verificar as configurações já estabelecidas, digite o comando abaixo.

	git config --list

Se os seus dados cadastrados não estão mais corretos, dê os seguintes comandos para removê-los.

- Nome do autor

		git config --global --unset user.name

- E-mail do autor

		git config --global --unset user.email

Dados esses comandos, o próximo passo seria seguir o exemplo que quem nunca configurou o Git, ou seja, quem está usado o Git pela primeira vez. Para isso, siga o exemplo abaixo para fazer essa configuração.

### Exemplo

> **NOTA:** Use os mesmos dados configurados no **GitHub**.

- Adicionar e-mail;

		git config --global user.email "seu e-mail"

> **global** é usado para que essa configuração seja usada em todos os seus próximos repositórios e não somente neste repositório.

- Adicionar o nome do autor;

		git config --global user.name "seu nome"

## Status do arquivo Git

Exibe o ***status*** do arquivo.

	git status

## Exemplo

- Pelo Git Bash, entre na pasta em que o Git foi iniciado;

- Execute o comando;

		git status

- Verifique o status dos arquivos.

## Iniciar o versionamento

Envia o arquivo para a área de **Staged (Palco)**.

	git add nome do arquivo

Envia todos os arquivos de uma única vez para a área **Staged (Palco)**.

	git add *

Abaixo esta uma outra forma de escrever o mesmo comando acima.

	git add .

Retira o arquivo da área de **Staged (Palco)**.

	git restore --staged nome do arquivo

## Criar um commit

Comando para **commitar** um arquivo que já está aguardando na área de **Staged (Palco)**.

	git commit

### Exemplo

	git commit -m "mensagem"

> Será usada uma ***flag*** **-m** para anexar uma mensagem ao **commit**.