# Guia simplificado

## 1 Configurações iniciais do Git


**Baixando e instalando o Git**
```bash
https://git-scm.com/downloads
```

**Configura nome de usuário**
```bash
git config --global user.name nome-sobrenome
```

**Configura email de usuário**
```bash
git config --global user.email email@email.com.br
```
---

</br>
</br>

## 2 Inicializando um repositório


**Inicializa o versionamento no respectivo diretório**
```bash
git init
```
---

<br>
<br>

## 3 Comandos básicos para sobreviver

**Verifica o status do repositório**
```bash
git status
```

**Adiciona todos os arquivos para serem commitados**
```bash
git add .
```

**Commitando arquivos**
```bash
git commit -m "[SWIFT-1] inserir um comentário significativo"

git commit -m "SWIFT-1 inserir um comentário significativo"
```

**Visualizando relatório de commits**
```bash
git log // todos os commits

git log --oneline // exibe log com hash e título do commit
```

**Adicionando um repositório remoto**
```bash
git remote add origin https://github.com/User/Repository.git
```

**Enviando as modificações para o repositório remoto**
```bash
git push origin <branch>
```

**Puxando alterações do repositório remoto**
```bash
git pull origin <branch>
```
---

<br>
<br>

## 4 Trabalhando com branchs

**Criando e locomovendo-se para uma nova branch**
```bash
git checkout -b nome-branch 
```

**Aplicando merge em branchs**
```bash
git merge nome-branch // precisa estar na branch de destino
```

**Visualizando todas as branches existentes no repositório**
```bash
git branch
```

**Deletando uma branch local**
```bash
git branch -D nome-branch
```

**Deletando uma branch remoto**
```bash
git push origin :nome-branch
```