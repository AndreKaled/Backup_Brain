# O básico
## Configurando identificação
`git config --global user.name "NomeDeUsuario"`
O comando salva em configuração global o nome de usuário, especificado entre os parênteses.

`git config --global user.email "email@email"`
O comando salva em configuração global o e-mail de usuário, especificado entre os parênteses.
## Criando repositórios 
`git init`
Inicializa git na pasta local, criando um arquivo .git com algumas configurações definidas. O git mostrará o nome da Branch principal em uso (normalmente Master)

`git branch -M main`
Altera a branch atual para a main, recomendado ao iniciar o Git, para garantir compatibilidade, diferente da master.


## Adicionando alterações ao repositório
`git status`
Revela o status atual dos arquivos, mostrando os arquivos rastreados pelo Git.

`git add name_file`
Adiciona o arquivo mencionado para ser rastreado pelo Git ao próximo commit.

`git add .`
Adiciona os arquivos da pasta para serem rastreados pelo Git ao próximo commit.

`git add *`
Adiciona todos os arquivos e subpastas da pasta atual para serem rastreados pelo Git ao próximo commit.

`git commit -m "mensagem de commit"`
Salva o conteúdo dos arquivos e a mensagem de registro do usuário, que descreve as alterações.

`git push`
Envia o commit ao repositório remoto.
## Clonando repositórios
`git clone <URL>`
Clona todo o projeto da URL na pasta atual.
A URL pode ser HTTP ou SSH.
## Atualizando repositório local
`git pull`
 Faz a busca e download do conteúdo do repositório remoto, para atualizar o repositório local e tornar os conteúdos iguais.
 Detalhe: `git pull` é a junção do `git fetch` e `git merge`.

---
# Conhecendo um pouco mais...
## Branches (Branch)
>Branch, é o nome dado para o sistema de versionamento que usamos através do Git e GitHub, para manter controle dos projetos.

A *Main* ou *Master* é a Branch principal do repositório, imagine-o como o tronco principal de um galho, contendo a versão mais estável e segura do código.
As outras Branches são galhos deste tronco, representam novas funcionalidades, correção de . Estas Branches podem se fundir novamente com a Branch principal.