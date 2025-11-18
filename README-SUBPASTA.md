# Mix Mateus - Versão para SUBPASTA

## 🎯 Esta versão funciona em `public_html/1/`

Esta é uma versão especial que usa **caminhos relativos** em vez de absolutos, permitindo que o site funcione dentro de uma subpasta.

---

## 📂 **ONDE COLOCAR OS ARQUIVOS:**

```
public_html/
└── 1/                          ← Sua subpasta
    ├── .htaccess               ← Configurado para /1/
    ├── index.html              ← Caminhos relativos
    ├── diagnostico.html        ← Ferramenta de teste
    ├── favicon.png
    ├── logo-mix-mateus.png
    └── assets/
        ├── index-BE-s8Z0w.css
        ├── index-CL0Mndgf.js
        └── Happy_couple_Mix_Mateus_card_approval_770ee240-CNrgi5Vf.png
```

**⚠️ IMPORTANTE:** Todos os arquivos devem estar DENTRO da pasta `1`, não na raiz do `public_html`.

---

## 🚀 **INSTRUÇÕES DE UPLOAD:**

### 1️⃣ **Baixar o ZIP**
https://github.com/Samuel151513/mix-mateus-landing-page/archive/refs/heads/main.zip

### 2️⃣ **Extrair**
Extraia TODOS os arquivos do ZIP

### 3️⃣ **Upload para `public_html/1/`**

Entre no Gerenciador de Arquivos da Hostinger:

1. Navegue até `public_html/1/`
2. **DELETE tudo** que estiver lá dentro
3. Faça upload de **TODOS** os arquivos extraídos para dentro de `1/`

### 4️⃣ **Corrigir Permissões**

Selecione todos os arquivos → Botão direito → Alterar Permissões:

- **Arquivos:** 644
- **Pasta `assets/`:** 755

### 5️⃣ **Testar**

Acesse:
- Site: `https://simuleaqui.online/1/`
- Diagnóstico: `https://simuleaqui.online/1/diagnostico.html`

Se TUDO ficar VERDE no diagnóstico, está funcionando! ✅

---

## 🔧 **O QUE MUDOU NESTA VERSÃO:**

### Caminhos Absolutos → Relativos

**ANTES (não funcionava em subpasta):**
```html
<link href="/favicon.png">
<script src="/assets/index-CL0Mndgf.js">
```

**AGORA (funciona em subpasta):**
```html
<link href="./favicon.png">
<script src="./assets/index-CL0Mndgf.js">
```

### .htaccess Configurado

```apache
RewriteBase /1/  # ← Aponta para a subpasta
```

---

## ✅ **CHECKLIST FINAL:**

Depois do upload, verifique:

- [ ] URL funciona: `https://simuleaqui.online/1/`
- [ ] Diagnóstico verde: `https://simuleaqui.online/1/diagnostico.html`
- [ ] Logo aparece no topo e rodapé
- [ ] Imagem do casal aparece
- [ ] Botão funciona (redireciona para Google)

---

## 🆘 **PROBLEMAS?**

### Página em branco?
1. Verifique se TODOS os arquivos estão em `public_html/1/`
2. Verifique permissões (644 para arquivos, 755 para pastas)
3. Limpe o cache: `Ctrl + Shift + R`

### Diagnóstico com erro vermelho?
1. Veja QUAL arquivo está faltando (CSS, JS, logo, etc)
2. Certifique-se que esse arquivo foi enviado
3. Verifique se a pasta `assets/` está completa

### Ainda não funciona?
Entre em contato com suporte da Hostinger:
- Telefone: 0800 006 5025
- Chat: https://www.hostinger.com.br/contato

---

**Versão:** 3.2 (Subpasta)  
**Data:** 18 de Novembro de 2025  
**Desenvolvido por:** Replit Agent
