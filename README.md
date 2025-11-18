# Landing Page Mix Mateus - Cartão de Crédito

## 📁 Estrutura do Projeto

```
github-deploy/
├── css/
│   ├── style.css    (77 KB - Estilos da aplicação)
│   └── app.js       (274 KB - JavaScript da aplicação)
├── fonts/
│   └── (vazio - fontes carregadas via Google Fonts)
├── images/
│   ├── favicon.png
│   ├── hero-casal.png         (1.3 MB - Imagem do casal Mix Mateus)
│   └── logo-mix-mateus.png    (321 KB - Logo Mix Mateus)
└── index.html
```

## 🚀 Como Fazer Upload no GitHub

### Opção 1: Via Interface Web do GitHub

1. **Crie um novo repositório no GitHub:**
   - Vá para https://github.com/new
   - Nome do repositório: `mix-mateus-landing-page` (ou o nome que preferir)
   - Deixe público ou privado conforme sua preferência
   - **NÃO** marque "Initialize with README"
   - Clique em "Create repository"

2. **Faça upload dos arquivos:**
   - Na página do repositório vazio, clique em "uploading an existing file"
   - Arraste todos os arquivos e pastas da pasta `github-deploy`
   - Ou clique em "choose your files" e selecione tudo
   - Escreva uma mensagem de commit (ex: "Initial commit - Landing Page Mix Mateus")
   - Clique em "Commit changes"

### Opção 2: Via Git CLI (Linha de Comando)

Se você tem Git instalado localmente:

```bash
# Entre na pasta github-deploy
cd github-deploy

# Inicialize o repositório Git
git init

# Adicione todos os arquivos
git add .

# Faça o primeiro commit
git commit -m "Initial commit - Landing Page Mix Mateus"

# Conecte ao seu repositório remoto (substitua SEU_USUARIO e SEU_REPO)
git remote add origin https://github.com/SEU_USUARIO/SEU_REPO.git

# Faça o push
git branch -M main
git push -u origin main
```

## 🌐 Ativar GitHub Pages

Depois de fazer upload:

1. Vá nas **Settings** do repositório
2. No menu lateral, clique em **Pages**
3. Em "Source", selecione:
   - Branch: `main`
   - Folder: `/ (root)`
4. Clique em **Save**
5. Aguarde alguns minutos e seu site estará disponível em:
   `https://SEU_USUARIO.github.io/SEU_REPO/`

## ✨ Funcionalidades

- **Botão "SOLICITAR MEU CARTÃO AGORA"**: Redireciona para https://google.com
- **Botão "SOLICITAR AGORA"**: Mostra notificação "Em breve!"
- **Design responsivo**: Funciona em mobile, tablet e desktop
- **Imagem customizada**: Casal com cartão Mix Mateus azul

## 📝 Notas

- Total do site: ~2 MB (imagens otimizadas)
- Compatível com todos os navegadores modernos
- Sem dependências externas (exceto Google Fonts via CDN)
- Pronto para SEO com meta tags configuradas

## 🔧 Manutenção

Para atualizar o site:
1. Edite os arquivos localmente
2. Faça upload novamente no GitHub
3. Ou use Git para fazer commit e push das mudanças

---

**Desenvolvido para Mix Mateus S.A. - 2025**
