# CHAVE SSH PELO SISTEMA WINDOWS

## Primeiro passo pelo GitHub

- Entrar no **[GitHub](https://github.com/)**;

- Criar uma conta GitHub ou entrar em sua conta;

- Clicar na setinha ao lado do ícone na parte superior direita da sua tela;

- Clicar em [**Settings**](https://github.com/settings/profile) (Configurações);

- Entre em [**SSH and GPG keys**](https://github.com/settings/keys) (Chaves SSH e GPG);

- Vá para o **segundo passo**.

## Segundo passo pelo Git Bash (CLI - Command-line interface)

- Execute o comando;

		ssh-keygen -t ed25519 -c seu e-mail

- Mostrará o local que a chave será salva, copie esse caminho e dê **"Enter"**;

- Pedirá uma **passphrase** (senha), coloque sua senha, entretanto, não aparecerá a senha sendo digitada, mas está.

- Vai pedir para repetir a sua senha, digite-a mais uma vez;

- Em um arquivo de texto ou mesmo na barra do navegador, altere esse caminho que você copiou anteriormente e copie;

	- Caminho copiado anteriormente:
  
			/c/Users/seu usuário/.ssh/id_ed25519

	- Retire a parte final e adicione o comando **"cd"**, copie o caminho:

			cd /c/Users/seu usuário/.ssh/

- Volte lá no Git Bash e cole esse comando;

- Para listar e visualizar o que está dentro desta pasta, utilize o comando abaixo;

		ls

- Use o comando a seguir para poder visualizar o contéudo da chave pública;

		cat id_ed25519.pub

- Copie a chave pública que será mostrada na tela. Ela será uma soma de **ssh-ed25519, letras e números e, por fim, seu e-mail**;

- Volte ao GitHub.

## Terceiro passo no GitHub

- De volta na tela das [**SSH and GPG keys**](https://github.com/settings/keys) (Chaves SSH e GPG);

- Clique em **New SSH key** (Nova chave SSH);

- Em **title** (título), coloque um nome qualquer para identificar o seu computador;

- Em **key** (chave), cole a chave pública copiada lá no Git Bash;

- Pressione em **Add SSH key** (Adicionar chave SSH);

- Volte para o Git Bash.

## Quarto passo pelo Git Bash (CLI - Command-line interface)

- Verifique se você ainda está dentro da pasta correta usando o comando;

	- Comando de verificação:

			pwd

	- Pasta correta:

			/c/Users/nome do usuário/.ssh


- Se você ainda estiver dentro da pasta correta vá para o próximo passo, caso não esteja, execute o comando abaixo;

		cd /c/Users/seu usuário/.ssh/

- Digite o comando a seguir;

		eval $(ssh-agent -s)

- Vai gerar um número de **Agent pid**;

- Execute o seguinte comando para passar para o **agent pid** a sua chave privada;

		ssh-add id_ed25519

- Vai te pedir a sua senha, digite-a e dê **Enter**;

- Vai retornar com uma mensagem de que a identificação foi adicionada;

- **CHAVE SSH ADICIONADA!**