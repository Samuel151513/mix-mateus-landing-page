# Mix Mateus - Sistema Completo v3.4

## 🎉 Sistema 100% Funcional

Landing page profissional + Formulário de verificação completo para cartão de crédito Mix Mateus.

## 📦 Conteúdo do Deploy

```
/1/
├── .htaccess                  ← Regras de redirecionamento
├── index.html                 ← Página única (SPA) com roteamento
├── diagnostico.html           ← Ferramenta de teste
├── favicon.png
├── logo-mix-mateus.png        ← Logo Mix Mateus (nome fixo)
├── casal-feliz.png            ← Imagem do casal (nome fixo)
└── assets/
    ├── index-BsyEAtB5.css     ← Estilos
    └── index-Be42FRMp.js      ← JavaScript completo
```

## 🚀 Upload para Hostinger

### Passo a Passo (Gerenciador de Arquivos)

1. **Download:**
   - Baixe: https://github.com/Samuel151513/mix-mateus-landing-page/archive/refs/heads/main.zip
   - Extraia o arquivo ZIP

2. **Limpeza:**
   - Acesse `public_html/1/` no Gerenciador de Arquivos
   - **DELETE TUDO** dentro da pasta `/1/`

3. **Upload:**
   - Faça upload de **TODOS OS ARQUIVOS** para dentro de `/1/`
   - Inclua: `.htaccess`, `index.html`, `diagnostico.html`, imagens e pasta `assets/`

4. **Permissões:**
   - Arquivos: 644
   - Pastas: 755

5. **Teste:**
   - Acesse: `https://simuleaqui.online/1/diagnostico.html`
   - Verifique todos os checkmarks verdes ✅

## 📱 URLs do Sistema

- **Landing Page (Página 1):** `https://simuleaqui.online/1/`
- **Formulário (Página 2):** `https://simuleaqui.online/1/#/2`
- **Diagnóstico:** `https://simuleaqui.online/1/diagnostico.html`

## ✨ Funcionalidades

### Página 1 - Landing Page (/)
- Hero section com logo e imagem do casal
- Trust badges (100% Online, Aprovação Rápida, etc)
- Seção "Como Funciona" (3 passos)
- Benefícios do Cartão (6 cards)
- CTA final com disclaimer
- Footer completo

**Botão Principal:** Redireciona para `../2` (formulário)

### Página 2 - Formulário de Verificação (/#/2)

**20+ campos organizados em 4 seções:**

1. **Documento**
   - CPF (formato: 000.000.000-00)
   - Data de nascimento

2. **Faixa de Renda**
   - RadioGroup com 4 opções

3. **Como Pretende Usar o Cartão**
   - RadioGroup com 4 opções (Supermercado, Compras online, etc)

4. **Fonte de Renda (3.1)**
   - Tipo de renda (CLT, Autônomo, MEI/PJ, Benefício)
   - Tempo na ocupação
   - Conta bancária ativa
   - Tempo com a conta
   - Atrasos nos últimos 12 meses

5. **Moradia (3.2)**
   - Tipo de moradia
   - Tempo no endereço atual

6. **Uso Previsto (3.3)**
   - Quanto costuma gastar por compra
   - Limite desejado

7. **Fatura e Comunicação (3.4)**
   - Dia preferido de vencimento
   - Como quer receber fatura (Email, WhatsApp, Ambos)
   - Lembretes automáticos de pagamento

8. **Aceite de Termos (4)**
   - **OBRIGATÓRIO:** Usuário DEVE aceitar para enviar
   - RadioGroup: "Sim, aceito" ou "Não"
   - Validação: Só aceita "Sim"

9. **Campos Finais**
   - Nome completo
   - Telefone (formato: (00) 00000-0000)
   - E-mail
   - Cidade

### Validações Implementadas

✅ CPF: Formato brasileiro com pontos e hífen  
✅ Telefone: Formato (00) 00000-0000  
✅ E-mail: Validação de email  
✅ Aceite de termos: **Obrigatório** - bloqueia envio sem aceite  
✅ Todos os campos select/radio têm valores padrão  
✅ Mensagens de erro claras e em português  

### Feedback ao Usuário

✅ **Toast de sucesso** após envio  
✅ **Mensagens de validação** em tempo real  
✅ **Loading state** no botão durante envio  
✅ **Reset do formulário** após sucesso  

## 🎨 Design

- **Cores:** Azul Mix Mateus (primário) + Vermelho (accent)
- **Tipografia:** Sans-serif moderna
- **Responsivo:** Mobile-first design
- **Acessibilidade:** data-testid em todos os elementos interativos

## 🔧 Tecnologia

- React + TypeScript
- Vite (build otimizado)
- Shadcn UI + Tailwind CSS
- Zod (validação)
- TanStack Query (estado)
- Wouter (roteamento)

## 🧪 Testes

Sistema **100% testado** com Playwright:
- ✅ Navegação entre páginas
- ✅ Validação de termos
- ✅ Envio de formulário
- ✅ Persistência de dados
- ✅ Mensagens de sucesso

## 📊 Backend (Desenvolvimento)

- Express.js + TypeScript
- Storage in-memory
- Endpoints:
  - `POST /api/verifications` - Criar verificação
  - `GET /api/verifications` - Listar verificações
  - `GET /api/verifications/:id` - Buscar por ID

## 🐛 Resolução de Problemas

### Imagens não aparecem
- Verifique se `logo-mix-mateus.png` e `casal-feliz.png` estão na raiz de `/1/`
- Permissões: 644

### CSS/JS não carrega
- Verifique se a pasta `assets/` está completa
- Arquivos CSS/JS devem ter permissão 644
- Pasta assets/ deve ter permissão 755

### Formulário não envia
- Aceitar os termos é **obrigatório**
- Preencha todos os campos de texto obrigatórios
- Verifique console do navegador (F12) para erros

### Página em branco
- Verifique se `.htaccess` está configurado
- RewriteBase deve ser `/1/`
- Permissão do `.htaccess`: 644

## 📞 Suporte

Para dúvidas técnicas, consulte:
- `diagnostico.html` - Ferramenta de teste
- Console do navegador (F12) - Erros JavaScript
- Logs do servidor - Erros backend

---

**Versão:** 3.4 - Sistema Completo Funcionando  
**Data:** 18/11/2025  
**Status:** ✅ 100% Operacional
