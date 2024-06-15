# O básico
## Configurando identificação
> git config --global user.name "NomeDeUsuario">
 
O comando salva em configuração global o nome de usuário, especificado entre os parênteses.

> git config --global user.email "email@email">

O comando salva em configuração global o email de usuário, especificado entre os parênteses.
## Criando repositórios 
> git init Inicializa git na pasta local, criando um arquivo .git com algumas configurações definidas. O git mostrará o nome da Branch principal em uso (normalmente Master)

>git branch -M main

Altera a branch atual para a main, recomendado ao iniciar o git, para garantir compatibilidade, diferente da master.
