[[Git]]
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
## Manipulando branch
`git branch`
Lista todas as branches do repositório local.

`git branch -a`
Lista todas as branches locais e remotas.

`git branch -r`
Lista todas as branches remotas.

`git branch --merged`
Lista todas as branches já mescladas com a **main**.

`git branch --no-merged`
Lista todas as branches **não** mescladas com a **main**.

`git checkout <branch_name>`
Muda para a branch especificada.

`git branch <branch_name>`
Cria uma nova branch.

`git fetch`
Atualiza as branches locais, sem mesclar as alterações.

`git merge <branch_name>`
Mescla/Integra as alterações da branch especificada à branch atual.

`git branch -d <branch_name>` ou `git branch -D <branch_name>
Deleta a branch especificada.

`git branch -m <branch_name> <new_branch_name>`
Renomeia o nome da branch.

`git push`
Envia a branch local para o repositório remoto.

`git push origin <branch_name>`
Envia a branch especificada para o origin.

`git branch --compare <branch_name> <branch_name2>`
Compara diferenças entre as branches.

`git log <branch_name>`
Mostra o histórico de commits da branch especificada.

`git reset --hard <branch_name>`
Exclui todos os commits da branch, retorna para o commit inicial.

#Git 