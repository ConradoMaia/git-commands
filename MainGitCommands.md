
# Git Commands Documentation

## 1. `git init`
Inicializa um novo repositório Git.

**Uso:**
```bash
git init
```

- Sem parâmetros.
- **Obrigatório:** Não.

---

## 2. `git clone`
Clona um repositório remoto para a máquina local.

**Uso:**
```bash
git clone <url> [diretório]
```

- `<url>`: URL do repositório a ser clonado. **Obrigatório.**
- `[diretório]`: Nome do diretório para o repositório clonado. **Opcional.**

---

## 3. `git status`
Mostra o estado atual da árvore de trabalho (modificações, arquivos prontos para commit, etc.).

**Uso:**
```bash
git status
```

- Sem parâmetros.
- **Obrigatório:** Não.

---

## 4. `git add`
Adiciona arquivos ao índice (staging area).

**Uso:**
```bash
git add <arquivo>
```

- `<arquivo>`: Arquivo ou diretório a ser adicionado ao índice. **Obrigatório.**
- `.`: Adiciona todos os arquivos modificados no diretório atual. **Opcional.**

---

## 5. `git commit`
Grava as mudanças no repositório com uma mensagem descritiva.

**Uso:**
```bash
git commit -m "<mensagem>"
```

- `-m "<mensagem>"`: Mensagem descritiva do commit. **Obrigatório.**
- `-a`: Adiciona todos os arquivos modificados e os inclui no commit. **Opcional.**
- `--amend`: Modifica o último commit (muito usado para corrigir mensagens de commit). **Opcional.**

---

## 6. `git log`
Exibe o histórico de commits.

**Uso:**
```bash
git log
```

- Sem parâmetros.
- **Obrigatório:** Não.

Parâmetros opcionais:
- `--oneline`: Exibe o histórico de commits de forma compacta.
- `--graph`: Exibe o histórico com um gráfico de branches e merges.

---

## 7. `git branch`
Lista, cria ou deleta branches.

**Uso:**
```bash
git branch
git branch <nome-branch>
```

- Sem parâmetros: lista todas as branches. **Opcional.**
- `<nome-branch>`: Cria uma nova branch. **Opcional.**
- `-d <nome-branch>`: Deleta uma branch. **Opcional.**

---

## 8. `git checkout`
Muda para uma branch específica ou restaura arquivos.

**Uso:**
```bash
git checkout <nome-branch>
git checkout <arquivo>
```

- `<nome-branch>`: Muda para a branch especificada. **Obrigatório** se estiver mudando de branch.
- `<arquivo>`: Restaura um arquivo específico do índice. **Opcional.**

---

## 9. `git merge`
Mescla uma branch com outra.

**Uso:**
```bash
git merge <nome-branch>
```

- `<nome-branch>`: Nome da branch a ser mesclada na branch atual. **Obrigatório.**

---

## 10. `git pull`
Atualiza o repositório local com as mudanças do repositório remoto e faz merge.

**Uso:**
```bash
git pull [<remoto>] [<branch>]
```

- `<remoto>`: Nome do repositório remoto (padrão é `origin`). **Opcional.**
- `<branch>`: Nome da branch a ser baixada. **Opcional.**

---

## 11. `git push`
Envia os commits locais para o repositório remoto.

**Uso:**
```bash
git push [<remoto>] [<branch>]
```

- `<remoto>`: Nome do repositório remoto (padrão é `origin`). **Opcional.**
- `<branch>`: Nome da branch a ser enviada. **Opcional.**

---

## 12. `git fetch`
Baixa os objetos e refs do repositório remoto sem fazer merge.

**Uso:**
```bash
git fetch [<remoto>] [<branch>]
```

- `<remoto>`: Nome do repositório remoto (padrão é `origin`). **Opcional.**
- `<branch>`: Nome da branch a ser baixada. **Opcional.**

---

## 13. `git reset`
Reseta o índice e a árvore de trabalho para o estado do último commit.

**Uso:**
```bash
git reset [--soft | --mixed | --hard] [<commit>]
```

- `--soft`: Mantém as mudanças no índice. **Opcional.**
- `--mixed`: Mantém as mudanças na árvore de trabalho (padrão). **Opcional.**
- `--hard`: Desfaz todas as mudanças, tanto no índice quanto na árvore de trabalho. **Opcional.**
- `<commit>`: Especifica até qual commit deve ser resetado. **Opcional.**

---

## 14. `git rebase`
Reaplica commits em cima de outra base de commits.

**Uso:**
```bash
git rebase <branch>
```

- `<branch>`: Nome da branch onde os commits serão reaplicados. **Obrigatório.**

---

## 15. `git stash`
Salva mudanças temporárias na árvore de trabalho sem fazer commit.

**Uso:**
```bash
git stash
```

- Sem parâmetros.
- **Obrigatório:** Não.

Parâmetros opcionais:
- `git stash pop`: Aplica as mudanças salvas no stash.
- `git stash list`: Lista os stashes salvos.
- `git stash drop`: Remove um stash salvo.

---

## 16. `git tag`
Cria, lista ou deleta tags.

**Uso:**
```bash
git tag <nome-tag>
```

- `<nome-tag>`: Nome da tag a ser criada. **Obrigatório** se estiver criando uma nova tag.
- `-d <nome-tag>`: Deleta a tag especificada. **Opcional.**
- `-a <nome-tag> -m "<mensagem>"`: Cria uma tag anotada com uma mensagem. **Opcional.**

---

## 17. `git remote`
Gerencia repositórios remotos.

**Uso:**
```bash
git remote
git remote add <nome> <url>
```

- Sem parâmetros: lista os repositórios remotos configurados. **Opcional.**
- `add <nome> <url>`: Adiciona um novo repositório remoto com o nome e URL especificados. **Obrigatório** para adicionar um repositório.

---

## 18. `git diff`
Exibe as diferenças entre commits, branches ou o estado da árvore de trabalho.

**Uso:**
```bash
git diff [<commit>] [<arquivo>]
```

- `<commit>`: Especifica o commit para comparar. **Opcional.**
- `<arquivo>`: Especifica o arquivo a ser comparado. **Opcional.**

---

## 19. `git revert`
Reverte um commit específico, criando um novo commit que desfaz as mudanças.

**Uso:**
```bash
git revert <commit>
```

- `<commit>`: Hash do commit a ser revertido. **Obrigatório.**

---

## 20. `git blame`
Mostra quem fez cada alteração em um arquivo linha por linha.

**Uso:**
```bash
git blame <arquivo>
```

- `<arquivo>`: Arquivo a ser analisado. **Obrigatório.**

---
