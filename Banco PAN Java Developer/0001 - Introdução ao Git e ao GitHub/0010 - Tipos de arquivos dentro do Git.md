# TIPOS DE ARQUIVO DENTRO DO GIT

## Untracked (Não rastreado)

O Git **não conhece** ainda esse arquivo.

## Tracked (Rastreado)

O Git **já conhece** esse arquivo.

### Unmodified (Não modificado)

Esse arquivo já é conhecido pelo Git, mas ele ainda não sofreu modificações, ou seja, já foi **commitado**.

> É um **commit**.

## Modified (Modificado)

Esse arquivo já é conhecido pelo Git, porém sofreu alterações **após** ser **commitado**. Isso significa que o Git ainda não conhece as alterações feitas.

## Staged (Palco)

Essa é a última fase antes de um arquivo ou mais ser **commitado**. Essa fase tem relação direta com dois tipos de arquivos já comentados aqui.

- Untracked (Não rastreado);

- Modified (Modificado).

Para que um arquivo ou mais entre no radar do Git pela primeira vez, será necessário excutar o seguinte comando.

	git add nome do arquivo

- Para adicionar mais de um arquivo de uma única vez;

      git add*

- Variação do mesmo comando acima.

      git add .

Do mesmo modo, arquivos que já haviam sido **commitados**, passaram para a fase **não modicado (unmodified)** e, em seguida, foram **modificados (modified)**, deverão usar o mesmo comando acima para ir para a fase **staged**.

# COMMIT

São as versões do seu arquivo, ou seja, todas as suas modificações desde da primeira versão até a final. É a etapa posterior a **staged** em que, após o **commit** ser realizado, o arquivo volta a ser **não modificado (unmodified)**.

- Para **commitar** um arquivo ou mais.

      git commit nome do arquivo

## AMBIENTES DE DESENVOLVIMENTO

## Working directory (Diretório de trabalho)

Literalmente o diretório de trabalho, onde os arquivos estão sendo trabalhados, onde as modificações estão sendo feitas.

## Staging area (Área de preparação)

Área onde os seus arquivos estão esperando para serem **commitados**. Está relacionada com a fase **staged (palco)** comentada anteriormente.

## Local repository (Repositório local)

Arquivos já **commitados** e guardados no seu computador.

# SERVIDOR

## Remote repository (Repositório remoto)

É onde os arquivos são enviados para serem guardados em nuvem. Um exemplo disso é o próprio **GitHub**.