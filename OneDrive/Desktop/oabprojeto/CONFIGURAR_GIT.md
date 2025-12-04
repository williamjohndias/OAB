# ⚙️ Configurar Git e Fazer Push

## ✅ Passos para Configurar

### 1. Configurar seu nome e email (JÁ FEITO)

```powershell
git config --global user.name "Seu Nome"
git config --global user.email "seu-email@example.com"
```

**Substitua pelos seus dados reais!**

### 2. Fazer o commit (JÁ FEITO)

```powershell
git commit -m "Initial commit: Sistema de consulta às Leis Orgânicas de Curitiba"
```

### 3. Criar repositório no GitHub

1. Acesse: https://github.com/new
2. Nome: `consulta-leis-organicas-curitiba` (ou outro)
3. **NÃO marque** "Add a README"
4. Clique em "Create repository"

### 4. Conectar e fazer push

**Substitua `SEU_USUARIO` pelo seu usuário do GitHub:**

```powershell
git remote add origin https://github.com/SEU_USUARIO/consulta-leis-organicas-curitiba.git
git push -u origin main
```

**⚠️ IMPORTANTE:** Use `git push` (não apenas `push`)

### 5. Se pedir credenciais

- **Usuário:** Seu usuário do GitHub
- **Senha:** Use um **Personal Access Token** (não sua senha normal)

#### Como criar Personal Access Token:

1. GitHub → Settings → Developer settings
2. Personal access tokens → Tokens (classic)
3. Generate new token (classic)
4. Marque: `repo` (acesso completo)
5. Copie o token gerado
6. Use como senha

---

## 🔄 Comandos Completos (Copie e Cole)

```powershell
# 1. Configurar Git (substitua pelos seus dados)
git config --global user.name "Seu Nome"
git config --global user.email "seu-email@example.com"

# 2. Fazer commit (se ainda não fez)
git add .
git commit -m "Initial commit: Sistema de consulta às Leis Orgânicas de Curitiba"

# 3. Renomear branch para main
git branch -M main

# 4. Adicionar remote (SUBSTITUA SEU_USUARIO)
git remote add origin https://github.com/SEU_USUARIO/consulta-leis-organicas-curitiba.git

# 5. Fazer push
git push -u origin main
```

---

## ✅ Verificar se Funcionou

Acesse seu repositório:
```
https://github.com/SEU_USUARIO/consulta-leis-organicas-curitiba
```

Você deve ver todos os arquivos!

---

## 🆘 Problemas Comuns

### "remote origin already exists"
```powershell
git remote remove origin
git remote add origin https://github.com/SEU_USUARIO/nome-repo.git
```

### "Permission denied"
- Use Personal Access Token ao invés de senha
- Verifique se o token tem permissão `repo`

### "fatal: not a git repository"
```powershell
git init
```

---

**Pronto!** 🎉

