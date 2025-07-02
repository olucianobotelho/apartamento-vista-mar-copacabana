# 🚀 Instruções de Deploy - Apartamento Vista Mar Copacabana

## 📋 Pré-requisitos
- Conta no GitHub
- Conta no Vercel
- Git instalado localmente

## 🔧 Passo 1: Criar Repositório no GitHub

### Método Manual (Recomendado)
1. **Acesse GitHub**: [https://github.com](https://github.com)
2. **Clique em "New repository"** (botão verde)
3. **Configure o repositório**:
   - **Repository name**: `apartamento-vista-mar-copacabana`
   - **Description**: `Landing page moderna para apartamento vista mar em Copacabana`
   - **Visibility**: Public (para deploy gratuito no Vercel)
   - **NÃO** marque "Add a README file" (já temos um)
   - **NÃO** adicione .gitignore (já temos um)
   - **License**: MIT (opcional)
4. **Clique em "Create repository"**

## 🔗 Passo 2: Conectar Repositório Local

### Execute os comandos no terminal:
```bash
# Adicionar remote origin (substitua SEU-USUARIO pelo seu username)
git remote add origin https://github.com/SEU-USUARIO/apartamento-vista-mar-copacabana.git

# Verificar se o remote foi adicionado
git remote -v

# Enviar código para o GitHub
git push -u origin main
```

### Exemplo com username real:
```bash
# Se seu username for "joaosilva"
git remote add origin https://github.com/joaosilva/apartamento-vista-mar-copacabana.git
git push -u origin main
```

## 🌐 Passo 3: Deploy no Vercel

### Método GitHub (Automático)
1. **Acesse Vercel**: [https://vercel.com](https://vercel.com)
2. **Faça login** com sua conta GitHub
3. **Clique em "New Project"**
4. **Import Git Repository**:
   - Selecione o repositório `apartamento-vista-mar-copacabana`
   - Clique em "Import"
5. **Configure o projeto**:
   - **Project Name**: `apartamento-vista-mar-copacabana`
   - **Framework Preset**: Other
   - **Root Directory**: `./`
   - **Build Command**: (deixe vazio)
   - **Output Directory**: (deixe vazio)
   - **Install Command**: (deixe vazio)
6. **Clique em "Deploy"**

### Método CLI (Alternativo)
```bash
# Instalar Vercel CLI
npm i -g vercel

# Fazer deploy
vercel

# Seguir as instruções interativas
```

## 🎯 Passo 4: Configurar Domínio (Opcional)

### No painel do Vercel:
1. **Acesse o projeto** deployado
2. **Vá em "Settings" > "Domains"**
3. **Adicione um domínio customizado** (se tiver)
4. **Configure DNS** conforme instruções

## ✅ Verificação Final

### Checklist de Deploy:
- [ ] Repositório criado no GitHub
- [ ] Código enviado com `git push`
- [ ] Deploy realizado no Vercel
- [ ] Site acessível via URL do Vercel
- [ ] Funcionalidades testadas:
  - [ ] Navegação por gestos nas fotos
  - [ ] Botão WhatsApp aparece ao rolar
  - [ ] Layout responsivo
  - [ ] Footer visível

## 🔧 Comandos Úteis

### Atualizações futuras:
```bash
# Fazer alterações no código
# Adicionar mudanças
git add .

# Commit com convenção Angular
git commit -m "feat: nova funcionalidade"
# ou
git commit -m "fix: correção de bug"
# ou
git commit -m "style: ajustes visuais"

# Enviar para GitHub (deploy automático no Vercel)
git push
```

### URLs Importantes:
- **GitHub**: `https://github.com/olucianobotelho/apartamento-vista-mar-copacabana`
- **Vercel**: `https://apartamento-vista-mar-copacabana.vercel.app`
- **Local**: `http://localhost:8000`

## 🆘 Solução de Problemas

### Erro: "remote origin already exists"
```bash
git remote remove origin
git remote add origin https://github.com/SEU-USUARIO/apartamento-vista-mar-copacabana.git
```

### Erro: "failed to push"
```bash
git pull origin main --allow-unrelated-histories
git push -u origin main
```

### Deploy falhou no Vercel
- Verifique se todos os arquivos estão no repositório
- Confirme que o `vercel.json` está configurado corretamente
- Verifique logs de build no painel do Vercel

---

**🎉 Parabéns! Seu apartamento vista mar agora está online!**