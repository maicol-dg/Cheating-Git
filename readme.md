

Cheating Git:

1. [`Configurações Iniciais`](/WebDevStudios/Custom-Metaboxes-and-Fields-for-WordPress/wiki/Field-Types#title)





#### `Configurações Iniciais`


```
git config --global user.name "Nome"
git config --global user.email "email@email.com"
```


#### `Criando Git Local`

Navegue até a pasta onde você pretende criar seu projeto e inicie o Git
```
git init
```


#### `Verificando Status Git`

```
git status
```


#### `Adicionando todos arquivos para commit`

```
git add .
```


#### `Commit arquivos`

```
git commit -m "Mensagem do Commit"
```


#### `Adicionar e Commit, ao mesmo tempo`

```
git commit -a -m "Mensagem Commit"
```


#### `Ignorando arquivos`

Para ignorar arquivos basta criar um arquivo chamado .gitignore e dentro adicionar os nomes dos aquivos que deseja ignorar, e para pastas acrescentar / ao final do nome
```
.gitignore
humans.txt
_old/
```


#### `Listar alterações de arquivos`

```
git diff
```


#### `Listando Commit`

```
git log
```


```
git log --pretty=oneline
```


#### `Visualizando interface gráfica Git`

```
gitk
```


#### `Atualizando ultimo commit, primeiro adicione o arquivo manualmente`

```
git add .
```


Agora só Commitar
```
git commit --amend -m "Commit a ser editado"
```


#### `Tirar arquivos antes de Commitar`

```
git reset HEAD nome_arquivi=o.php
```


#### `Voltando versão do arquivo`

```
git checkout -- nome_arquivo.php
```


#### `Remover arquivos do diretórios`

```
git rm nome_arquivo.php
```


#### `Criando TAG`

```
git tag -a nome_tag -m "Mensagem TAG"
```


#### `Listando TAG`

```
git tag
```


#### `Criando TAG para um determinado Commit`

Primeiro listamos os commits
```
git log --pretty=oneline
```


Após listar os commits, pegaremos a chave do commit e adicionamos a TAG
```
git tag -a nome_tag chave_commit -m "Mensagem TAG"
```


#### `Ver detalhes TAG`

```
git show nome_tag
```


#### `Deletando TAG`

```
git tag -d nome_tag
```


#### `Criando ambiente (branch)`

```
git branch nome_branch
```


#### `Listando Branch`

```
git branch
```


#### `Usando Branch`

```
git checkout nome_branch
```


#### `Mesclando versões git`

Acesse o branch master e mescle com outro branch
```
git merge nome_branch
```


#### `Deletando Branch`

```
git branch -d nome_branch
```


#### `Criando Git Servidor`

Navegue onde você deseja criar seu git server, para ser clonado
```
git init --bare
```


#### `Clonando repositório server`

clonando do servidor
```
git clone file:////caminho/seu/repositorio
```


#### `Clonando do servidor (remoto) para seu local`

```
git clone git+ssh://user@192.168.25.100/caminho/server/repositorio nome_pasta_que_sera_criado
```


<a href="http://wiki.pipa.digital/criando-projeto-git-no-servidor-e-clonando-projeto/">Saiba Mais Aqui!</a>

#### `Enviando Clone para o servidor`

```
git push origin master
```


#### `Atualizando alterações, e mesclando arquivos`

```
git pull origin master
```


#### `Avisando desenvolvedor de alterações, sem mesclar`

```
git fetch origin nome_branch
```

