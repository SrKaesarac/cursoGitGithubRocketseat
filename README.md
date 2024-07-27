# Curso de Git e Github da Rocketseat

## Comandos básicos do Git:

### git init

```
Para iniciar um repositório vazio do Git.
```  

### git status 
```
Para verificar a situação dos arquivos presentes no repositório.
```

### git add `<nomeDoArquivo>`
```
Para adicionar um arquivo na "staging area" onde o arquivo passará a ser monitorado e terá um ponto na história do repositório local. 

O arquivo adicionado com o git add possui uma versão armazenada, e quaisquer alterações após o comando git add, precisam ser adicionadas a staging area com um novo git add para atualizar as mudanças.
 
```

### git add .
```
Para adicionar todos os arquivos presentes no repositório, para a staging area.
```

### git rm --cached `<nome do arquivo>` 
```
Para remover um arquivo da staging area. Aquela versão que havia sido armazenada na staging area deixará de existir.rm significa "remove" e --cached pois o arquivo está na Staging Area, que é armazenada em Cache local.
```

### git restore `<nome do arquivo>`
```
Para restaurar um arquivo para seu antigo ponto na história, no caso o último ponto de salvamento antes das mudanças.
```

### git commit -m "mensagem do commit" 
```
Para fazer um Commit, ou seja, registrar uma versão de seu trabalho atual, criando um ponto na história. o "-m" serve para o git saber que o que vem a seguir é uma mensagem do commit.
```

### git pull 
```
Puxa as modificações do repositório remoto para o local.
```

### git push 
```
Envia as modificações locais para o repositório remoto.
```

### git checkout -b `<nome da nova branch>` 
```
Para criar uma nova branch, muito útil para criações de novas funcionalidades sem interferir no fluxo de trabalho da branch principal "Main". o -b serve para o git saber que se trata da criação de uma branch nova.
```
### git checkout `<nome da branch>` 
```
Para trocar de uma branch para outra já existente.
```

### git log 
```
Para visualizar todos os dados recentes sobre commits e alterações.
```

### :
```
Para sair da tela de log 
```

### git checkout `<ID do commit>` 
```
Para "entrar" no commit. A partir desse comando todas as alterações feitas existirão apenas localmente, dentro do ponto da história referente aquele Commit. 

Você ainda pode fazer novos commits, mas para incorporá-los ao código é necessário criar uma nova branch com o seguinte comando. 

Ótima forma de recuperar arquivos deletados caso eles tenham sido commitados em algum momento, basta usar o comando:

    git checkout <id> -- nomeDoArquivo 

E o arquivo terá sido recuperado.
```

### git switch -c `<nome da nova branch>` 
```
Para commitar as alterações feitas a partir de um Commit.
```
### git switch - 
```
Para desfazer o comando anterior de git switch.
```
### git clone `<chave https do repositorio>` 
```
Para clonar um repositorio do GitHub para seu git local.
```

## Como conectar o Git local ao GitHub:
```
git remote add origin git@github.com:nomeDoUsuario/nomeDoRepositorio.git
git branch -M main
git push -u origin main
```
## Como usar o GitHub para modificar arquivos e commitar:

     Pressione o botão ponto final " . " dentro da pagina principal do repositorio que deseja acessar.
     Você será transportado para uma interface do GitHub semelhante ao VSCode que lhe permitirá fazer algumas alterações sem rodar o código e com suporte para Commits e branches.