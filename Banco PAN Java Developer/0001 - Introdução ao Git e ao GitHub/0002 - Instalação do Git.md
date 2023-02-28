# INSTALAÇÃO DO GIT

## Windows

- [Link de download](https://git-scm.com/)

## Linux e Unix

- [Link de download](https://git-scm.com/download/linux);
- Verificar o sabor de Linux;
- Usar o comando para a versão mais recente do Git.

### Exemplo

- Sabor: **Debian/Ubuntu**;

	- add-apt-repository ppa:git-core/ppa

	- apt update; apt install git;
      
- Chamar o comando. Foi usado uma flag "y" para fazer a confirmação automaticamente quando o comando for chamado;

      sudo add-apt-repository ppa:git-core/ppa -y

- Para fazer a atualização para a versão mais recente do Git;

      sudo apt update

- Instala o Git.

      sudo apt install git

	- Pode aparecer um mensagem de confirmação, dar "Y" para "sim".

## Verfificar a versão do git

    git --version

## O que é "sudo"?

A primeira coisa que temos que entender é o “sudo”. O sudo é um utilitário de linha de comando para permitir usuários normais a executarem outros utilitários com permissões mais elevadas, de acordo com as suas regras. Ou seja, o sudo controla os acessos dos usuários normais ao super-usuário do sistema, também conhecido como root.

O su é apenas um comando para trocar de usuário. O “s” significa “swich” e o “u” significa “user”, isto é, “switch user” (trocar de usuário). O objetivo de colocar o “sudo” como antecedente, é porque o “su” já vai ser executado como super-usuário, trocando o usuário da sessão atual para o “root”.

$ sudo su # Muda para o usuário root

$ su mateus # Muda para o usuário mateus

$ su maria # Muda para o usuário maria

Perceba que apenas para o root é diferente, pois o “sudo” já eleva a permissão.

## macOS

- Instalar o "Homebrew";

- Colar o comando.

      brew install git