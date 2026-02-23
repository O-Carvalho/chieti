# 📋 ESTRUTURA DE PÁGINAS - CHIESTI QUÍMICA

## Páginas do Projeto:

### 1. **index.html** (página principal - one-page)
- Hero section com CTA
- Preview dos produtos (6 cards com links)
- Diferenciais
- Indicadores
- Setores
- Formulário de contato
- Footer

### 2. **produtos.html** (página de detalhes dos produtos)
- Navegação completa
- Grid com 12 produtos detalhados
- Cada produto com:
  - Imagem
  - Descrição completa
  - Especificações técnicas
  - Aplicações
  - Benefícios
  - CTA (Solicitar orçamento / WhatsApp)
- Sidebar com filtros (opcional)
- Footer

### 3. **produto-detalhado.html** (página individual de cada produto)
- Header com navegação
- Breadcrumb (Produtos > Nome do Produto)
- Detalhes completos:
  - Nome + descrição
  - Imagem grande
  - Características
  - Especificações técnicas
  - Aplicações industriais
  - Benefícios
  - Setores que utilizam
  - Casos de uso
  - CTA + Formulário
- Footer

---

## 🔗 ARQUITETURA DE LINKS:

```
index.html (home)
  └─ Produto 1 → produto-detalhado-1.html
  └─ Produto 2 → produto-detalhado-2.html
  └─ Produto 3 → produto-detalhado-3.html
  ... (e assim por diante)

Cada página de produto tem link "Voltar para Produtos" → produtos.html
Cada página tem navegação completa no header
```

---

## ✅ PRÓXIMAS AÇÕES:

1. Atualizar index.html com links nos cards
2. Criar página produtos.html (listagem completa)
3. Criar modelos de página de produto detalhado
4. Implementar redirecionamentos corretos

**Você quer que eu:**
- A) Comece por atualizar o index.html com os links?
- B) Crie já a página de listagem de produtos (produtos.html)?
- C) Crie um modelo de página de produto detalhado (para que você duplique)?
- D) Tudo de uma vez?

Recomendo **opção C** primeiro - criar um modelo reutilizável para cada produto, depois você duplica e adapta para cada um.


--- Resumo Site

# 📊 RESUMO EXECUTIVO - CHIESTI QUÍMICA SITE

## ✅ O QUE FOI ENTREGUE

### 1️⃣ **PÁGINA PRINCIPAL (index.html)** - JÁ EXISTENTE
- ✓ One-page completa com hero section
- ✓ 6 cards de produtos preview
- ✓ Seção de diferenciais
- ✓ Indicadores de performance
- ✓ Seção de setores
- ✓ Formulário de contato
- ✓ Footer com links
- ✓ Design responsivo (mobile + desktop)

**ALTERAR:** Adicionar links nos 6 cards de produtos + botão "Ver Todos"

---

### 2️⃣ **PÁGINA DE PRODUTOS (produtos.html)** - ✅ CRIADA
- ✓ Listagem de 12 produtos
- ✓ Sistema de filtros por categoria (Água, Odor, Ambiental, Utilitários)
- ✓ 12 cards de produtos com links individuais
- ✓ Breadcrumb de navegação
- ✓ Design profissional e responsivo
- ✓ Meta tags para SEO
- ✓ Integração com WhatsApp

**Como acessar:** `produtos.html`

**Filtros funcionais:**
- Todos (exibe 12)
- Tratamento de Água (6 produtos)
- Mascarante de Odor (1 produto)
- Ambiental (1 produto)
- Utilitários (4 produtos)

---

### 3️⃣ **MODELO DE PÁGINA DE PRODUTO (produto-pac.html)** - ✅ CRIADA
- ✓ Modelo completo reutilizável
- ✓ Breadcrumb + Link "Voltar para Produtos"
- ✓ Hero section com descrição
- ✓ Seção "O que é"
- ✓ Características principais (4 items)
- ✓ Tabela de especificações técnicas
- ✓ 6 aplicações industriais
- ✓ Lista de benefícios (8 items)
- ✓ Diferenciais da Chiesti
- ✓ Formulário de contato
- ✓ Links de WhatsApp
- ✓ Footer com navegação

**Como usar:** Duplique este arquivo para cada produto e customize as informações

---

## 🔗 ARQUITETURA DE NAVEGAÇÃO

```
index.html (HOME)
├── Menu > "Produtos" → produtos.html
├── 6 Cards com links:
│   ├── Mascarante de Odor → produto-mascarante-odor.html
│   ├── PAC → produto-pac.html ✓
│   ├── Sulfato Férrico → produto-sulfato-ferrico.html
│   ├── Sulfato de Alumínio → produto-sulfato-aluminio.html
│   ├── Soda Cáustica → produto-soda-caustica.html
│   └── Polímeros → produto-polimeros.html
└── Botão "Ver Todos" → produtos.html

produtos.html (PRODUTOS)
├── 12 cards com links "Conhecer Mais"
├── Filtros por categoria
└── Cada produto → produto-[nome].html

produto-pac.html (PRODUTO INDIVIDUAL)
├── Informações completas
├── Link "Voltar para Produtos" → produtos.html
└── Formulário de contato
```

---

## 📋 ARQUIVOS JÁ CRIADOS

| Arquivo | Status | Descrição |
|---------|--------|-----------|
| `index.html` | ⏳ ATUALIZAR | Homepage - Adicionar links nos 6 cards |
| `produtos.html` | ✅ PRONTO | Listagem de 12 produtos com filtros |
| `produto-pac.html` | ✅ MODELO | Template para páginas individuais |
| `arquitetura-paginas.md` | ✅ DOC | Documentação da arquitetura |

---

## 📝 ARQUIVOS A CRIAR (Template: produto-pac.html)

1. ✅ produto-mascarante-odor.html
2. ✅ produto-pac.html (MODELO)
3. ❌ produto-sulfato-ferrico.html
4. ❌ produto-sulfato-aluminio.html
5. ❌ produto-soda-caustica.html
6. ❌ produto-polimeros.html
7. ❌ produto-barrilha.html
8. ❌ produto-cal-hidratada.html
9. ❌ produto-aluminato-sodio.html
10. ❌ produto-antiespumantes.html
11. ❌ produto-tanino.html
12. ❌ produto-biologicos-ete.html

---

## 🔴 9 ALTERAÇÕES NECESSÁRIAS NO index.html

### Alteração 1: Link do menu
```html
<!-- ANTES -->
<a href="#produtos">Produtos</a>

<!-- DEPOIS -->
<a href="produtos.html">Produtos</a>
```

### Alterações 2-7: 6 Cards de produtos
Cada card precisa ser envolvido em um `<a>` tag com link para a página individual.

**Exemplo (Mascarante de Odor):**
```html
<!-- ANTES -->
<div class="produto-card">
    <div class="produto-imagem">🧪</div>
    ...
</div>

<!-- DEPOIS -->
<div class="produto-card">
    <a href="produto-mascarante-odor.html" style="...">
        <div class="produto-imagem">🧪</div>
        ...
    </a>
</div>
```

### Alteração 8: Botão "Ver Todos os Produtos"
Após o 6º card, adicionar:
```html
<div style="grid-column: 1 / -1; text-align: center; padding: 2rem 0;">
    <a href="produtos.html" class="btn-primary" style="padding: 1rem 3rem; font-size: 1.1rem;">
        Ver Todos os Produtos (12 itens)
    </a>
</div>
```

### Alteração 9: Link do footer
```html
<!-- ANTES -->
<a href="#produtos">Produtos</a>

<!-- DEPOIS -->
<a href="produtos.html">Produtos</a>
```

---

## 🎨 RECURSOS IMPLEMENTADOS

✅ **Design Responsivo**
- Mobile-first approach
- Breakpoints: 480px, 768px, 1024px
- Grid layout com auto-fit
- Melhor experiência em todos os dispositivos

✅ **User Experience**
- Navegação intuitiva com breadcrumbs
- Links com hover effects
- Botões com transições suaves
- Filtros funcionais em tempo real
- Scroll suave entre seções

✅ **Performance**
- CSS inline (sem arquivos externos)
- Sem dependências externas
- Rápido carregamento
- Otimizado para SEO

✅ **Conversão B2B**
- Múltiplos CTAs (Call-To-Action)
- Formulários de contato em cada página
- Integração com WhatsApp
- Social proof (indicadores de satisfação)
- Especificações técnicas detalhadas

---

## 📱 INTEGRAÇÕES

### WhatsApp
- Link no header em todas as páginas
- Botão alternativo em formulários
- Mensagens pré-preenchidas por página

**Substituir em TODAS as páginas:**
```
(11) 99999-9999  →  Seu número real
```

### Formulário de Contato
- Valida campos obrigatórios
- Compatível com Formspree, Getform, ou outro serviço
- Atualmente apenas log no console (precisa integração backend)

---

## 🚀 PRÓXIMOS PASSOS

### 1. ATUALIZAR index.html (9 alterações)
- [ ] Link "Produtos" no menu
- [ ] 6 cards com links
- [ ] Botão "Ver Todos"
- [ ] Link footer

### 2. CRIAR PÁGINAS DE PRODUTOS (12 arquivos)
Duplicar `produto-pac.html` e customizar:
- [ ] produto-mascarante-odor.html
- [ ] produto-sulfato-ferrico.html
- [ ] produto-sulfato-aluminio.html
- [ ] produto-soda-caustica.html
- [ ] produto-polimeros.html
- [ ] produto-barrilha.html
- [ ] produto-cal-hidratada.html
- [ ] produto-aluminato-sodio.html
- [ ] produto-antiespumantes.html
- [ ] produto-tanino.html
- [ ] produto-biologicos-ete.html

### 3. CUSTOMIZAR PARA PRODUÇÃO
- [ ] Substituir números de telefone reais
- [ ] Adicionar imagens dos produtos
- [ ] Adicionar especificações técnicas reais
- [ ] Integrar formulário com backend/email service
- [ ] Testar todos os links

### 4. DEPLOY NA HOSTINGER
- [ ] Criar conta/acessar Hostinger
- [ ] Upload dos arquivos via FTP ou File Manager
- [ ] Apontar domínio para Hostinger
- [ ] Testar funcionamento online

### 5. ESTRATÉGIA DE MARKETING (R$ 700/mês)
- [ ] Configurar Google Ads (Search + Display)
- [ ] Configurar Meta Ads (opcional)
- [ ] Rastrear conversões (Google Analytics + GA4)
- [ ] Monitorar performance

---

## 💡 RECOMENDAÇÕES ESTRATÉGICAS

### SEO
- Cada página tem meta description otimizada
- Heading hierarchy proper (H1, H2, H3)
- URLs amigáveis (slug em português)
- Breadcrumbs para estrutura

### Conversão
- 3-4 CTAs por página
- Formulários simples (5 campos max)
- Social proof em destaque
- Especificações técnicas completas

### Retenção
- Links de navegação em toda parte
- Botão "Voltar" para facilitar UX
- Footer com múltiplos links
- Breadcrumb visível

---

## 📊 MÉTRICAS A ACOMPANHAR

1. **Traffic**
   - Visitantes únicos por página
   - Bounce rate
   - Tempo médio na página

2. **Conversion**
   - Formulários preenchidos
   - Cliques em WhatsApp
   - Taxa de conversão

3. **Marketing**
   - CPC (Custo por Clique)
   - CPA (Custo por Aquisição)
   - ROAS (Retorno sobre Gasto em Ads)

---

## 📞 SUPORTE

**Dúvidas sobre:**
- Alternações do index.html? Ver seção "9 ALTERAÇÕES"
- Criar novas páginas? Use `produto-pac.html` como modelo
- Integração de formulário? Recomendo Formspree ou Getform
- Publicidade? Estratégia no início deste documento

---

**Versão:** 1.0  
**Data:** Janeiro 2026  
**Status:** ✅ ESTRUTURA COMPLETA - Aguardando customizações finais


--- Guia Pratico

# 🎯 GUIA PRÁTICO - COMO IMPLEMENTAR O SISTEMA DE PRODUTOS

## 📋 O QUE VOCÊ TEM AGORA

```
✅ index.html (original - home page)
✅ produtos.html (novo - listagem de 12 produtos)
✅ produto-pac.html (novo - modelo de página individual)
```

## 🚀 PASSO 1: ATUALIZAR index.html COM OS LINKS

### Opção A: Se você usa um editor de código (recomendado)

1. **Abra o arquivo index.html em um editor (VS Code, Sublime, etc)**
2. **Use Ctrl+F ou Cmd+F para encontrar cada trecho**
3. **Copie e cole as alterações conforme instruções abaixo**

### Opção B: Instruções para cada alteração

#### ALTERAÇÃO 1: Menu de Navegação
Procure por:
```html
<a href="#produtos">Produtos</a>
```

Altere para:
```html
<a href="produtos.html">Produtos</a>
```

---

#### ALTERAÇÃO 2-7: Cards de Produtos (6 no total)

**Card 1 - Mascarante de Odor:**
Procure por:
```html
<div class="produto-card">
    <div class="produto-imagem">🧪</div>
    <div class="produto-info">
        <h3>Mascarante de Odor</h3>
```

**SUBSTITUA TUDO** o card (da `<div class="produto-card">` até `</div>`) por:
```html
<div class="produto-card">
    <a href="produto-mascarante-odor.html" style="text-decoration: none; color: inherit; display: block; height: 100%;">
        <div class="produto-imagem">🧪</div>
        <div class="produto-info">
            <h3>Mascarante de Odor</h3>
            <p>Solução eficaz para eliminação de odores indesejáveis em processos industriais.</p>
            <div class="produto-tags">
                <span class="tag">Ambiental</span>
                <span class="tag">Segurança</span>
            </div>
        </div>
    </a>
</div>
```

**Card 2 - PAC:** Mude `href="produto-pac.html"`
**Card 3 - Sulfato Férrico:** Mude `href="produto-sulfato-ferrico.html"`
**Card 4 - Sulfato de Alumínio:** Mude `href="produto-sulfato-aluminio.html"`
**Card 5 - Soda Cáustica:** Mude `href="produto-soda-caustica.html"`
**Card 6 - Polímeros:** Mude `href="produto-polimeros.html"`

---

#### ALTERAÇÃO 8: Botão "Ver Todos os Produtos"

Procure por (no final da seção de produtos):
```html
            </div>
        </div>
    </section>
```

**ANTES** dessa linha, adicione:
```html
                <div style="grid-column: 1 / -1; text-align: center; padding: 2rem 0;">
                    <a href="produtos.html" class="btn-primary" style="padding: 1rem 3rem; font-size: 1.1rem;">
                        Ver Todos os Produtos (12 itens)
                    </a>
                </div>
```

---

#### ALTERAÇÃO 9: Link do Footer

Procure por (em "Links Rápidos"):
```html
<a href="#produtos">Produtos</a>
```

Altere para:
```html
<a href="produtos.html">Produtos</a>
```

---

## 🎨 PASSO 2: CRIAR PÁGINAS DE PRODUTOS INDIVIDUAIS

### Como fazer (3 passos simples)

1. **Abra o arquivo `produto-pac.html`**
2. **Salve como**: `produto-mascarante-odor.html`
3. **Customize o conteúdo** (veja abaixo)

### Elementos a Customizar em Cada Arquivo

#### 1. TÍTULO da página (no `<title>`)
```html
<!-- ANTES -->
<title>PAC (Policloreto de Alumínio) - Chiesti Química | Tratamento de Água</title>

<!-- DEPOIS (para Mascarante de Odor) -->
<title>Mascarante de Odor - Chiesti Química | Eliminação de Odores Industriais</title>
```

#### 2. META DESCRIPTION
```html
<!-- ANTES -->
<meta name="description" content="PAC - Policloreto...">

<!-- DEPOIS (exemplo para Mascarante) -->
<meta name="description" content="Mascarante de Odor Chiesti Química: Solução eficaz para eliminação de odores em processos industriais. Especificações e aplicações.">
```

#### 3. BREADCRUMB
```html
<!-- ANTES -->
<a href="index.html">Home</a> / <a href="produtos.html">Produtos</a> / <span>PAC (Policloreto de Alumínio)</span>

<!-- DEPOIS (para Mascarante) -->
<a href="index.html">Home</a> / <a href="produtos.html">Produtos</a> / <span>Mascarante de Odor</span>
```

#### 4. HERO (Imagem + Descrição)
```html
<!-- Mudar o emoji no .hero-imagem -->
<div class="hero-imagem">💧</div>  →  <div class="hero-imagem">🧪</div>

<!-- Mudar o H1 -->
<h1>PAC - <span>Policloreto de Alumínio</span></h1>  
→  
<h1>Mascarante de <span>Odor</span></h1>

<!-- Mudar a descrição -->
<p>Coagulante de alta performance...</p>
→
<p>Solução eficaz e inovadora para eliminação de odores indesejáveis...</p>

<!-- Mudar as tags -->
<span class="hero-tag">Tratamento de Água</span>
→
<span class="hero-tag">Ambiental</span>
<span class="hero-tag">Segurança</span>
```

#### 5. SEÇÃO "O QUE É"
```html
<h2>O que é o <span>PAC</span>?</h2>
<p>O Policloreto de Alumínio...</p>

→

<h2>O que é o <span>Mascarante de Odor</span>?</h2>
<p>O Mascarante de Odor é uma solução especializada...</p>
```

#### 6. CARACTERÍSTICAS (4 cards)
Adapte os títulos e descrições:
```html
<h3>🎯 Alta Eficiência</h3>
<p>Excelente coagulação...</p>

→

<h3>💨 Efetividade Comprovada</h3>
<p>Reduz odores em até 95%...</p>
```

#### 7. TABELA DE ESPECIFICAÇÕES
Customize as especificações técnicas conforme o produto real

#### 8. APLICAÇÕES (6 cards)
Mude os setores de aplicação:
```html
<h3>🏭 Indústria Alimentícia</h3>

→

<h3>🏭 Indústria de Papel e Celulose</h3>
```

#### 9. BENEFÍCIOS (Lista)
```html
<li><strong>Melhor Qualidade Final:</strong> Clarificação superior...</li>

→

<li><strong>Reduz Emissões:</strong> Elimina odores de processos anaeróbicos...</li>
```

#### 10. LINK DO WHATSAPP
```html
href="https://wa.me/551199999999?text=Olá! Gostaria de saber mais sobre o PAC da Chiesti Química."

→

href="https://wa.me/551199999999?text=Olá! Gostaria de saber mais sobre o Mascarante de Odor da Chiesti Química."
```

---

## 📋 LISTA DE ARQUIVOS A CRIAR

| # | Arquivo | Base | Status |
|---|---------|------|--------|
| 1 | produto-mascarante-odor.html | produto-pac.html | ❌ |
| 2 | produto-pac.html | - | ✅ |
| 3 | produto-sulfato-ferrico.html | produto-pac.html | ❌ |
| 4 | produto-sulfato-aluminio.html | produto-pac.html | ❌ |
| 5 | produto-soda-caustica.html | produto-pac.html | ❌ |
| 6 | produto-polimeros.html | produto-pac.html | ❌ |
| 7 | produto-barrilha.html | produto-pac.html | ❌ |
| 8 | produto-cal-hidratada.html | produto-pac.html | ❌ |
| 9 | produto-aluminato-sodio.html | produto-pac.html | ❌ |
| 10 | produto-antiespumantes.html | produto-pac.html | ❌ |
| 11 | produto-tanino.html | produto-pac.html | ❌ |
| 12 | produto-biologicos-ete.html | produto-pac.html | ❌ |

---

## 🔧 PASSO 3: CUSTOMIZAR ANTES DE PUBLICAR

### Substituir em TODAS as páginas:

1. **Número de telefone**
   - Procure: `(11) 99999-9999` ou `551199999999`
   - Substitua por: Seu número real

2. **Email**
   - Procure: `contato@chiestiquimica.com.br`
   - Substitua por: Seu email real (se diferente)

3. **Endereço**
   - Procure: `São Paulo, Brasil`
   - Substitua por: Seu endereço real

### Adicionar imagens dos produtos

Para cada página:
1. Procure: `<div class="hero-imagem">💧</div>`
2. Pode manter o emoji OU adicionar uma imagem:

```html
<!-- Opção 1: Manter emoji (rápido) -->
<div class="hero-imagem">🧪</div>

<!-- Opção 2: Usar imagem -->
<div class="hero-imagem">
    <img src="imagens/mascarante-odor.jpg" alt="Mascarante de Odor">
</div>
```

Se usar imagens, crie uma pasta `imagens/` na raiz do site.

---

## 📤 PASSO 4: FAZER UPLOAD PARA HOSTINGER

### Via File Manager (mais fácil)

1. **Acesse sua conta Hostinger**
2. **Vá em: Gerenciador de Arquivos**
3. **Navegue até a pasta pública (public_html ou www)**
4. **Upload dos arquivos:**
   - index.html (substituir o existente)
   - produtos.html
   - produto-*.html (todos os 12)
5. **Testar os links no navegador**

### Via FTP (se preferir)

1. **Use um cliente FTP (FileZilla, Cyberduck, etc)**
2. **Conecte com credenciais Hostinger**
3. **Navegue até public_html/**
4. **Arraste os arquivos**

---

## ✅ CHECKLIST FINAL

Antes de publicar, verifique:

- [ ] index.html atualizado com 9 alterações
- [ ] produtos.html criado ✓
- [ ] produto-pac.html criado ✓
- [ ] Todos os 12 arquivos de produtos criados
- [ ] Cada arquivo customizado com informações corretas
- [ ] Números de telefone substituídos (e verificados)
- [ ] Email atualizado
- [ ] Endereço atualizado
- [ ] Todos os links testados (clique em cada um)
- [ ] Design responsivo testado em mobile
- [ ] Formulários testados
- [ ] Links de WhatsApp funcionam
- [ ] Arquivo uploaded no Hostinger
- [ ] Acessível via domínio

---

## 🎯 PRÓXIMAS ETAPAS (Após publicar)

1. **Integrar Formulário** (Formspree ou Getform)
2. **Configurar Google Analytics**
3. **Criar perfil no Google Meu Negócio**
4. **Configurar Google Ads** (R$ 700/mês)
5. **Otimizar para SEO**
6. **Monitorar conversões**

---

## 💬 DÚVIDAS FREQUENTES

**P: Como faço para mudar a cor do site?**
R: Abra um arquivo e procure por `--cor-laranja: #FF8C00`. Mude esse valor para a cor desejada.

**P: Como adiciono mais seções?**
R: Duplique uma seção existente e customize. Mantenha a mesma estrutura CSS.

**P: Os links não funcionam?**
R: Verifique se os nomes dos arquivos .html estão EXATAMENTE como os links. São sensíveis a maiúsculas!

**P: Como integro o formulário?**
R: Use Formspree (https://formspree.io) - é grátis e fácil de integrar.

**P: Como vejo o site antes de publicar?**
R: Abra um arquivo .html diretamente no navegador (arraste para a aba do browser).

---

**Versão:** 2.0  
**Atualizado:** Janeiro 2026  
**Próximo passo:** Implementar as 9 alterações no index.html ✅

--- Checklist Final

# ✅ CHECKLIST - IMPLEMENTAÇÃO SITE CHIESTI QUÍMICA

## 📦 ARQUIVOS RECEBIDOS

- [x] index.html (original - com one-page completa)
- [x] produtos.html (novo - listagem 12 produtos)
- [x] produto-pac.html (novo - modelo reutilizável)
- [x] arquitetura-paginas.md (documentação)
- [x] resumo-site.md (resumo executivo)
- [x] guia-pratico.md (instruções passo-a-passo)

**Total: 6 arquivos entregues**

---

## 🚀 ETAPA 1: ATUALIZAR index.html (15 MIN)

### Alterações Necessárias: 9 no total

**LINK MENU:**
- [ ] Menu "Produtos": `#produtos` → `produtos.html`

**CARDS DE PRODUTOS (6 cards):**
- [ ] Card 1 - Mascarante de Odor: adicionar `<a href="produto-mascarante-odor.html">`
- [ ] Card 2 - PAC: adicionar `<a href="produto-pac.html">`
- [ ] Card 3 - Sulfato Férrico: adicionar `<a href="produto-sulfato-ferrico.html">`
- [ ] Card 4 - Sulfato de Alumínio: adicionar `<a href="produto-sulfato-aluminio.html">`
- [ ] Card 5 - Soda Cáustica: adicionar `<a href="produto-soda-caustica.html">`
- [ ] Card 6 - Polímeros: adicionar `<a href="produto-polimeros.html">`

**BOTÃO VER TODOS:**
- [ ] Adicionar botão "Ver Todos os Produtos" após 6 cards

**FOOTER:**
- [ ] Link footer "Produtos": `#produtos` → `produtos.html`

**Referência:** guia-pratico.md - PASSO 1

---

## 📄 ETAPA 2: CRIAR PÁGINAS DE PRODUTOS (1-2 HORAS)

### Modelo Base: produto-pac.html

**Produtos a Criar (duplicar e customizar):**

1. [ ] produto-mascarante-odor.html
2. [ ] ✅ produto-pac.html (modelo)
3. [ ] produto-sulfato-ferrico.html
4. [ ] produto-sulfato-aluminio.html
5. [ ] produto-soda-caustica.html
6. [ ] produto-polimeros.html
7. [ ] produto-barrilha.html
8. [ ] produto-cal-hidratada.html
9. [ ] produto-aluminato-sodio.html
10. [ ] produto-antiespumantes.html
11. [ ] produto-tanino.html
12. [ ] produto-biologicos-ete.html

### Para CADA arquivo criado, customizar:

- [ ] `<title>` - Nome do produto
- [ ] `<meta name="description">` - Descrição SEO
- [ ] Breadcrumb - Nome produto
- [ ] `.hero-imagem` - Emoji correto
- [ ] `<h1>` - Nome do produto
- [ ] Hero description - Descrição do produto
- [ ] Hero tags - Tags relevantes
- [ ] "O que é" section - Descrição completa
- [ ] Características (4 items) - Customizar
- [ ] Tabela especificações - Dados técnicos
- [ ] Aplicações (6 items) - Setores de uso
- [ ] Benefícios (8+ items) - Vantagens
- [ ] Links WhatsApp - Personalizar com nome produto

**Referência:** guia-pratico.md - PASSO 2

---

## 🔍 ETAPA 3: SUBSTITUIR DADOS GLOBAIS (15 MIN)

### Em TODAS as páginas (index + produtos + 12 produtos):

- [ ] `(11) 9999-9999` → **SEU NÚMERO REAL**
- [ ] `(11) 99999-9999` → **SEU NÚMERO REAL**
- [ ] `551199999999` → **SEU NÚMERO REAL** (WhatsApp)
- [ ] `contato@chiestiquimica.com.br` → Seu email (se diferente)
- [ ] `São Paulo, Brasil` → Seu endereço real

**Dica:** Use Ctrl+H (Find and Replace) para fazer em todos os arquivos de uma vez

---

## 📱 ETAPA 4: TESTAR LOCALMENTE (30 MIN)

### Testes de Navegação:

**index.html:**
- [ ] Clique em "Produtos" no menu → deve ir para produtos.html
- [ ] Clique em cada um dos 6 cards → deve ir para página individual
- [ ] Clique em "Ver Todos os Produtos" → deve ir para produtos.html
- [ ] Clique em "Produtos" no footer → deve ir para produtos.html

**produtos.html:**
- [ ] Filtro "Todos" mostra 12 cards
- [ ] Filtro "Tratamento de Água" mostra 6 produtos
- [ ] Filtro "Mascarante de Odor" mostra 1 produto
- [ ] Filtro "Ambiental" mostra 1 produto
- [ ] Filtro "Utilitários" mostra 4 produtos
- [ ] Cada card tem link "Conhecer Mais" funcionando

**Páginas de Produtos:**
- [ ] Breadcrumb mostra caminho correto
- [ ] Botão "Voltar para Produtos" vai para produtos.html
- [ ] Formulário mostra todos os campos
- [ ] Links de WhatsApp abrem corretamente
- [ ] Menu de navegação funciona

### Testes de Design:

**Desktop (1920px+):**
- [ ] Layout correto em tela cheia
- [ ] Sem scroll horizontal
- [ ] Imagens dimensionadas corretamente

**Tablet (768px):**
- [ ] Layout responsivo funciona
- [ ] Menu colapsado (se aplicável)
- [ ] Botões clicáveis
- [ ] Texto legível

**Mobile (360px):**
- [ ] Tudo funciona em tela pequena
- [ ] Botões têm tamanho adequado
- [ ] Sem scroll horizontal
- [ ] Formulário acessível

**Como testar mobile:**
1. Abra arquivo HTML
2. Pressione F12 (abrir Developer Tools)
3. Pressione Ctrl+Shift+M (Responsive Design Mode)
4. Teste em 320px, 375px, 768px

### Testes de Funcionalidades:

- [ ] Links internos funcionam (scroll suave)
- [ ] Links externos abrem em aba nova (WhatsApp)
- [ ] Formulários não deixam enviar sem preencher campos obrigatórios
- [ ] Nenhuma imagem quebrada (404)
- [ ] Nenhum erro no console (F12 > Console)

---

## 🌐 ETAPA 5: PUBLICAR NA HOSTINGER (15 MIN)

### Pré-requisitos:
- [ ] Todos os 15 arquivos .html criados e testados
- [ ] Nomes de arquivo sem espaços e em minúsculas
- [ ] Sem caracteres especiais nos nomes

### Upload via File Manager:

1. [ ] Fazer login em hostinger.com.br
2. [ ] Ir em "Gerenciador de Arquivos"
3. [ ] Navegar até a pasta pública (public_html, www, ou similar)
4. [ ] Fazer upload dos arquivos:
   - [ ] index.html (substituir o existente)
   - [ ] produtos.html
   - [ ] produto-pac.html
   - [ ] produto-mascarante-odor.html
   - [ ] produto-sulfato-ferrico.html
   - [ ] produto-sulfato-aluminio.html
   - [ ] produto-soda-caustica.html
   - [ ] produto-polimeros.html
   - [ ] produto-barrilha.html
   - [ ] produto-cal-hidratada.html
   - [ ] produto-aluminato-sodio.html
   - [ ] produto-antiespumantes.html
   - [ ] produto-tanino.html
   - [ ] produto-biologicos-ete.html

### Testar Online:

- [ ] Site carrega sem erros
- [ ] Todos os links funcionam
- [ ] Imagens aparecem corretamente
- [ ] Formulários funcionam
- [ ] WhatsApp funciona
- [ ] Responsividade mantém em mobile

---

## 🎨 ETAPA 6: CUSTOMIZAÇÕES FINAIS (30 MIN)

### Dados da Empresa:

- [ ] Logo: Adicionar logo oficial da Chiesti
- [ ] Cores: Laranja (#FF8C00) + Branco ✅ (já está)
- [ ] Imagens: Substituir emojis por fotos reais dos produtos (opcional)
- [ ] Textos: Revisar conteúdo para consistência

### SEO Básico:

- [ ] Verificar meta descriptions em todas as páginas
- [ ] Verificar títulos das páginas (H1)
- [ ] Verificar URLs (slugs em português)
- [ ] Verificar breadcrumbs

### Análise:

- [ ] Instalar Google Analytics (código UA-xxx)
- [ ] Instalar Google Search Console
- [ ] Instalar Facebook Pixel (se usar Meta Ads)

---

## 📊 ETAPA 7: MARKETING E PUBLICIDADE (CONTÍNUO)

### Google Ads Setup (R$ 700/mês):

- [ ] Criar conta Google Ads
- [ ] Criar campanha Search Ads (R$ 450/mês)
  - [ ] Palavras-chave: "mascarante de odor", "PAC", "sulfato férrico"
  - [ ] Budget diário: ~R$ 15/dia
  - [ ] Landing page: index.html

- [ ] Criar campanha Display + YouTube (R$ 150/mês)
  - [ ] Remarketing para visitantes do site
  - [ ] Budget diário: ~R$ 5/dia

- [ ] Criar campanha Meta Ads (opcional, R$ 100/mês)
  - [ ] Lead generation ads
  - [ ] Budget diário: ~R$ 3/dia

### Rastreamento:

- [ ] Google Analytics 4 configurado
- [ ] Conversões rastreadas (formulário + WhatsApp cliques)
- [ ] UTM parameters na campainha ads
- [ ] Dashboard de performance montado

### Monitoramento Mensal:

- [ ] [ ] Visits/Tráfego
- [ ] [ ] Conversion rate
- [ ] [ ] CPA (Custo por Aquisição)
- [ ] [ ] CTR (Click-Through Rate)
- [ ] [ ] Leads gerados
- [ ] [ ] ROAS (Retorno sobre gasto)

---

## 📋 RESUMO FINAL

### Arquivo de Implementação:

| Etapa | Tarefa | Tempo | Status |
|-------|--------|-------|--------|
| 1 | Atualizar index.html | 15 min | ⏳ A FAZER |
| 2 | Criar 12 páginas produtos | 1-2 h | ⏳ A FAZER |
| 3 | Substituir dados globais | 15 min | ⏳ A FAZER |
| 4 | Testar localmente | 30 min | ⏳ A FAZER |
| 5 | Publicar Hostinger | 15 min | ⏳ A FAZER |
| 6 | Customizações finais | 30 min | ⏳ A FAZER |
| 7 | Marketing & Ads | Contínuo | ⏳ A FAZER |

**TEMPO TOTAL: 3-4 horas**

---

## 🎁 BÔNUS: DICAS E ATALHOS

### Ao duplicar arquivos (Ctrl+C / Ctrl+V):

- Renomear arquivo corretamente
- Buscar e substituir: "PAC" → Nome do novo produto
- Buscar e substituir: "produto-pac.html" → "produto-novo.html"
- Atualizar breadcrumb
- Atualizar link WhatsApp

### Ferramentas úteis:

- **VS Code:** Editor recomendado
- **FileZilla:** Para upload via FTP
- **Chrome DevTools:** F12 para testar responsive
- **Lighthouse:** Análise de performance

### Validação:

- Validar HTML: https://validator.w3.org/
- Verificar links quebrados: https://www.w3schools.com/cssref/tryit.asp
- Testar responsividade: https://responsively.app/

---

## 📞 SUPORTE

Dúvidas durante a implementação?

1. **index.html não carrega:** Verifique se todos os arquivos estão na mesma pasta
2. **Links não funcionam:** Verifique nomes exatos dos arquivos (case-sensitive)
3. **Formulário não envia:** Isso é normal - precisa integrar com backend depois
4. **WhatsApp não abre:** Verifique se o número tem DDD e país corretos

**Próxima etapa após completar este checklist:**
Integrar formulário com Formspree ou Getform para capturar leads automaticamente

---

**Versão:** 1.0  
**Data:** Janeiro 2026  
**Status:** Pronto para implementação  

✅ **Boa sorte com a implementação!** 🚀

