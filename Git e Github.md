# GIT E GITHUB

## Configurações iniciais

```git config --global user.name <your_name>``` = Define seu nome
```git config --global user.email <your_email>``` = Define seu email
```git config --global core.editor <your_editor>``` = Define seu editor
```git config --list``` = Lista suas configurações

## Começando com Repositório LOCAL
```sh git init``` = Inicia Repositório LOCAL
```git status``` = Retorna Status do Diretório

## Adicionando Arquivos ao Repositório Local
```git add <file_name>``` = Adiciona arquivo ao modo STAGE
```git add * ``` = Adiciona TODOS os arquivos ao modo STAGE
```git rm --cached <file_name>``` = Volta o arquivo no modo UNTRACKED

## Commitando Arquivos
```git commit -m "mensagem"``` = Versiona (Commita) o arquivo

## Mostrando Informações (LOGS)
```git log``` = Mostra os todos os arquivos e seus respectivos commits (Forma Detalhada)
```git shortlog``` = Mostra todos os arquivos e seus respectivos commits (Forma Reduzida)
```git show <commit_hash (código do commit)>``` = Mostra as informações do Commit de um arquivo específico

## Configurando Repositório REMOTO
```git remote add <repository_name> <caminho HTTPS ou SSH>``` = Inicia Repositório REMOTO
```git remote``` = Lista os Arquivos Remotos (Geral)
```git remote -v``` = Lista os Arquivos Remotos (Detalhado)
```git remote rm <repository_name>``` = Remove URL de um remote do Repositório

### Gerando SSH Key (Confirmar que você é o usuário):
-
1 - Abra o GIT Bash;
2 - Cole o seguinte comando:
```ssh-keygen -t rsa -b 4096 -C "your_email@example.com"``` = Cria uma nova SSH Key
id_rsa e id_rsa.pub serão gerados (SSH Keys)
3 - Ainda no GIT Bash, cole:
```cat id_rsa.pub```
4 - Copie a chave (SSH Key) que aparecer no terminal
5 - Acesse o Github
6 - Settings (Canto superior direito)
7 - Acesse 'SSH and GPG keys' (Canto esquerdo)
8 - Clique em 'New SSH key'
9 - Dê um titulo à sua Chave (Dica: Nome da sua máquina - Ex: 'Mackbook Pro' ou 'Home PC') em 'Title'
10 - Cole a chave (SSH Key) em 'Key'
11 - Clique 'Add SSH key'

obs: Caso não queira adicionar a SSH Key, existe um comando para Force Update (Sincroniza os arquivos igonorando e apagando arquivos já existentes):
```git push --set-upstream <repository_name> master -f``` (Não recomendado)
-

## Desfazendo alterações
```git checkout <file_name>``` = Desfaz última alteração do arquivo enviado ao Repositório REMOTO
```git reset HEAD <file_name>``` = Desfaz última alteração de arquivo enviado ao Repositório LOCAL

## Enviando Arquivos para o Repositório REMOTO
```git push -u <repository_name> master``` = Envia atualizações para o Repositório Remoto (SOMENTE Primeira Vez)
```git push``` = Envia atualizações para o Repositório Remoto (DEMAIS Vezes)

## Pegando Arquivos do Servidor REMOTO
```git pull``` = Pega arquivo e informações dos arquivos das pessoas trabalhando junto com você no mesmo Repositório e exibe (Dica: Use sempre antes de fazer qualquer alterações para atualizar os outros arquivos)
obs: Pega informação que está no REMOTE e trás para o LOCAL

## Mostrando Mudanças
```git diff``` = Mostra as mudanças feitas no arquivo (ANTES DO COMMIT)
```git diff --name-only``` = Mostra apenas os nomes dos arquivos que sofreram mudanças.

## Clone de Repositórios REMOTOS
Clonando Repositórios:
-
```git clone <Caminho HTTPS ou SSH>``` = Clona um repositório REMOTO.
obs: Sempre que utilizar o GIT CLONE, volte uma pasta do seu repositório local, pois uma nova pasta será criada.
-

### Glossário:
-
branch = Pacotes
commit = Gerar Versão (Versionar)
-

By Lip-ee
