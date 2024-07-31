## Comandos para trabalhar com repositório local
## Inicia um repositório local

```bash
git init
```
## verificar alterações de pastas e arquivos no projeto
```bash
git status
```
## Adiciona todos os arquivos e pastas modificados, ao stage area
```bash
git add
```
## Adiciona apenas o arquivo
```bash
git add frases.txt
```
## Deleta o arquivo do stage
```bash
git rm --cached .DS__store
```
## Restaura o arquivo original
```bash
git restore
```
## Cria e descreve um ponto na história
```bash
git commit -m "message here"
```
## Navegar pelos commits
```bash
git log
```
## Mudando HEAD de commit
```bash
git checkout 9b8dcd47e95f86 (ID)
```
## Voltar para o momento atual
```bash
git checkout master
```
## Histórico de commits do projeto
```bash
git log
```
## Recuperando um arquivo
Se eu deletar um arquivo, este, será rastreado pelo git.
Digitando o comando `git status`, você verá que o arquivo já está com status de "deletado" aguardando o comando `git add frases.txt` para adicionar no stage e fazer o commit.
```bash
// git checkout id -- nomedoarquivo
 git checkout 9b8dcd47e95f8 -- frases.txt
```
## Puxa modificações do repositório remoto para o repositório local
```bash
git pull
```
## Envia as modificações locais para o repositório remoto
```bash
git push
```
