### Merge de 3 vias com pull request

- obs tem o desenvolvedor que faz a branch ft-login e tem o desenvolvedor que faz a branch ft-pedidos



- vamos supor que outra pessoa esta trabalhano tambem no projeto, é o outro desenvolvedor, que vai fazer a branch ft-login:
faz um git clone desse projeto que esta no github, para puxar esse projeto do remoto e simular que outro desenvolvedor esta trabalhando nele.
esse desenvolvedor vai trabalhar nesse projeto agora, cria uma branch ft-login, depois vai para a branch com git checkout ft-login, coloca um codigo novo no vscode,
depois faz o git add . e o git commit, tudo na branch que ela esta trabalhando que é ft-login.
faz o git checkout main, para voltar pra branch main, e faz o git pull origin main para atualizar o local em relacao ao que esta no remoto, pra saber se ela nao esta desatualizada em relacao ao que ta no github.
vai para a branch que tava fazendo o projeto que é a branch git checkout ft-login, faz o merge do main para o login, e faz o git push -u origin ft-login para enviar o ft-login para o github.
agora a equipe olha no github e vai validar essa feature nova, atraves do pull request, e do merge desse pull request.
a equipe dando o ok, é feito o merge, vai juntar esse ft-login com a branch main.

- vamos agora com o desenvolvedor que faz a branch ft-pedidos:
cria a branch ft-pedidos com o codigo git branch ft-pedidos, depois muda para a branch para ft-pedidos, faz o comando git checkout ft-pedidos, e cria no vscode um codigo novo.
faz git add . e depois git commit, usa o comando git log --oneline, e observa que so tem os 2 commits do main e mais o commit que eu fiz agora que foi o de pagina de pedidos.
ou seja nao aparece os commits que o outro desenvolvedor fez anteriormente, que foi da branch ft-login.
crio mais 2 commits na minha branch que é ft-pedidos, pra isso fico dentro da minha branch ft-pedidos no gitbash, abro o vscode pra acrescentar algum codigo la, depois faço o git add . e git commit.
e faço git log --oneline pra saber do historico de att. 
agora vou pra branch main, e vou fazer o pull pra trazer o que ta la no github pra eu nao ficar desatualizado.
pode fazer o git log --oneline pra ver o historico e notamos que temos so os 2 commits la do main do github. ou seja nao temos o que o outro desenvolvedor da branch ft-pedidos fez ainda.
entao temos que fazer o pull para trazer do remoto para o local.
pronto agora meu local esta atualizado. faço git log --oneline pra ver que ja tem os commits que o colega criou e juntou la da branch ft-login para a branch main.
troco pra branch ft-pedidos
faço git merge main para puxar do main para o ft-pedidos
abre tela vim, clica esc, depois :q! para nao mudar o nome. ele mantem nome padrao para esse merge.
faço entao git log --oneline para ver o historico, percebo que esta na ordem cronologica as alteracoes no projeto.
agora mando para o github, com comando git push -u origin ft-pedidos
agora temos o pull request onde a equipe olha o me codigo e analisa se aprova, se o chefe aprovar, ele da o merge pull request. 

- pronto esta feito o passo a passo do merge de 3 vias com pull request.
