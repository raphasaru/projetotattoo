# Plano: Nova Landing Page - Projeto Tattoo

## Status: v1 IMPLEMENTADA

**Servidor:** `npm run dev` → http://localhost:4321/

---

## Resumo
Landing page de alta conversão para a escola Projeto Tattoo, com copy emocional focada em dores e desejos do público iniciante, CTAs para WhatsApp e integração com Google Sheets.

## Decisões Definidas
- **Preço:** Não mostrar na LP - revelar apenas no WhatsApp
- **Tom:** Equilíbrio entre emotivo/inspiracional e prático
- **Depoimentos:** Usar os existentes + sugestão de coletar mais
- **WhatsApp:** Usar mesmo link do site atual

---

## O QUE FOI IMPLEMENTADO

### Stack
- **Astro 5.x** - Framework estático ultra-rápido
- **CSS puro** - Sem dependências externas
- **Fontes:** Bebas Neue (display) + Outfit (body)
- **Cores:** Dark mode (#0a0a0a), Gold (#C9A962), Green (#22C55E)

### Componentes Criados (src/components/)
| Arquivo | Seção | Status |
|---------|-------|--------|
| Hero.astro | 1. Abertura emocional | OK |
| PainPoints.astro | 2. Agitação da dor | OK |
| Transformation.astro | 3. Ponte/solução | OK |
| SocialProof.astro | 4. Números de prova social | OK |
| Method.astro | 5. Timeline 4 semanas | OK |
| Testimonials.astro | 6. Depoimentos | OK |
| Portfolio.astro | 7. Galeria (placeholders) | OK |
| Investment.astro | 8. Potencial de ganhos | OK |
| Included.astro | 9. O que está incluso | OK |
| Objections.astro | 10. Quebra de objeções | OK |
| FAQ.astro | 11. Accordion FAQ | OK |
| FinalCTA.astro | 12. CTA urgência | OK |
| WhatsAppButton.astro | Botão flutuante | OK |
| PopupForm.astro | Pop-up captura leads | OK |

### Funcionalidades
- [x] 12 seções com copy emocional completa
- [x] CTAs verdes direcionando para WhatsApp
- [x] Botão WhatsApp flutuante (canto inferior direito)
- [x] Pop-up de captura após 15s (nome, email, telefone)
- [x] FAQ accordion funcional
- [x] Animações de entrada e hover
- [x] 100% responsivo (mobile-first)
- [x] SEO básico configurado

---

## PENDENTE / PRÓXIMOS PASSOS

### Configurações necessárias
1. **WhatsApp:** Substituir `5511999999999` pelo número real em:
   - Hero.astro
   - Transformation.astro
   - Method.astro
   - Investment.astro
   - FinalCTA.astro
   - WhatsAppButton.astro

2. **Google Sheets:** Configurar URL do Apps Script em PopupForm.astro

3. **Imagens:** Adicionar fotos reais em:
   - Portfolio.astro (galeria de trabalhos de alunos)
   - Testimonials.astro (fotos dos depoentes)
   - Hero.astro (imagem de tatuador)

### Melhorias futuras
- [ ] Adicionar analytics (GTM/GA4)
- [ ] Implementar exit intent no pop-up
- [ ] Adicionar mais depoimentos reais
- [ ] Otimizar imagens (WebP)
- [ ] Configurar domínio e deploy (Vercel/Netlify)

---

## Referências de UI (Google Stitch)

> **Adicionar prints aqui quando estiverem prontos**

<!--
Exemplo:
![Hero Section](./referencias/hero.png)
![Social Proof](./referencias/social-proof.png)
-->

---

## Stack Recomendada

**Astro** (framework estático)
- Zero JavaScript por padrão = páginas ultra-rápidas
- Excelente SEO out-of-the-box
- Build simples, deploy fácil (Vercel/Netlify gratuito)
- Perfeito para landing pages sem backend

**Estrutura do projeto:**
```
/
├── src/
│   ├── components/
│   │   ├── Hero.astro
│   │   ├── PainPoints.astro
│   │   ├── SocialProof.astro
│   │   ├── Method.astro
│   │   ├── Testimonials.astro
│   │   ├── Portfolio.astro
│   │   ├── Investment.astro
│   │   ├── Included.astro
│   │   ├── Objections.astro
│   │   ├── FAQ.astro
│   │   ├── FinalCTA.astro
│   │   ├── PopupForm.astro
│   │   └── WhatsAppButton.astro
│   ├── layouts/
│   │   └── Layout.astro
│   └── pages/
│       └── index.astro
├── public/
│   └── images/
├── astro.config.mjs
└── package.json
```

**Integração Google Sheets:** Via Google Apps Script (web app) - script simples que recebe POST do formulário.

---

## Estrutura da Página (12 seções)

### 1. HERO - Abertura Emocional
**Objetivo:** Capturar atenção com identificação imediata

**H1:**
> "Você sente que nasceu pra viver de arte, mas está preso numa vida que não é sua?"

**Subheadline:**
> Descubra como transformar sua paixão pela tatuagem em uma carreira lucrativa em apenas 1 mês — mesmo sem nunca ter desenhado na vida.

**CTA:** `[QUERO COMEÇAR MINHA TRANSFORMAÇÃO]` → WhatsApp

---

### 2. AGITAÇÃO - Amplificação da Dor
**Objetivo:** Fazer o visitante sentir suas frustrações

**H2:** "A cada domingo à noite, aquele aperto no peito volta..."

**Bullets de dor:**
- Você já se pegou no trabalho, olhando pela janela, imaginando como seria viver fazendo o que ama?
- Já sentiu inveja de quem trabalha com arte, enquanto você preenche planilhas sem fim?
- Já teve medo de que a vida passe e você nunca descubra do que realmente é capaz?

---

### 3. PONTE - A Transformação
**Objetivo:** Apresentar a solução

**H2:** "E se eu te dissesse que em 30 dias você pode estar tatuando de verdade?"

**Diferenciadores:**
- ✓ Pega na máquina desde o primeiro dia
- ✓ Tatua 4 pessoas REAIS durante o curso
- ✓ Sai com portfólio pronto pra começar a cobrar
- ✓ Entra numa comunidade de +5.000 tatuadores

---

### 4. PROVA SOCIAL - Números
**Objetivo:** Estabelecer autoridade

**Cards:**
| 12 Anos | +5.000 Alunos | +5M Views | +156K Seguidores | 7 Países |
|---------|---------------|-----------|------------------|----------|

---

### 5. MÉTODO - Como Funciona
**Objetivo:** Explicar o processo de forma tangível

**4 Semanas:**
1. **Fundamentos** - Biossegurança, equipamentos, primeiro contato com máquina
2. **Técnicas** - Linhas, preenchimento, sombreado, 1ª tatuagem real
3. **Aprofundamento** - Estilos, composição, 2ª e 3ª tatuagens
4. **Profissionalização** - Precificação, clientes, 4ª tatuagem, certificado

---

### 6. DEPOIMENTOS - Histórias Reais
**Objetivo:** Mostrar transformações com nome, foto e resultado

**Formato por depoimento:**
- Foto do aluno
- Nome + idade + profissão anterior
- Citação emocional
- Resultado atual (ex: "Studio próprio | R$12.000/mês")

**Nota:** Usar os depoimentos existentes. Recomendo coletar 2-3 histórias mais detalhadas de alunos que tiveram transformações marcantes (ex: mudança de carreira, abertura de estúdio).

---

### 7. PORTFOLIO - Galeria Visual
**Objetivo:** Demonstrar qualidade técnica

**H2:** "Trabalhos de quem começou do zero — assim como você"

Galeria 12-16 imagens de trabalhos de alunos

---

### 8. POTENCIAL DE GANHOS
**Objetivo:** Mostrar viabilidade financeira SEM revelar preço do curso

**H2:** "O investimento que se paga rápido"

**Cálculo visual do potencial:**
```
Quanto um tatuador iniciante cobra:
R$150-300 por tatuagem pequena

Se fizer apenas 3 tatuagens por semana:
R$1.800 a R$3.600/mês

Em 6 meses você pode estar faturando:
R$5.000 a R$10.000/mês
```

**CTA:** "Quero saber as condições" → WhatsApp (valores revelados apenas na conversa)

---

### 9. O QUE ESTÁ INCLUSO
**Objetivo:** Detalhar entregáveis

- ✓ 40 horas de imersão presencial
- ✓ 4 tatuagens em voluntários reais
- ✓ Kit de materiais para prática
- ✓ Certificado de conclusão
- ✓ Acesso vitalício à comunidade
- ✓ Lives mensais exclusivas

**Bônus:** Cursos extras de colorimetria e fotografia

---

### 10. OBJEÇÕES
**Objetivo:** Remover barreiras

| Objeção | Resposta |
|---------|----------|
| "Não sei desenhar" | 70% dos alunos nunca desenharam. Ensinamos técnicas específicas. |
| "Tenho medo de não conseguir" | Taxa de conclusão de 97% em 12 anos. |
| "É muito caro" | Alunos recuperam investimento em 4 semanas tatuando. |

---

### 11. CTA FINAL - Urgência
**Objetivo:** Converter

**H2:** "Sua transformação começa com uma decisão"

**Urgência:**
> ⚠️ ÚLTIMAS VAGAS - Turmas limitadas a 12 alunos

**CTA:** `[GARANTIR MINHA VAGA AGORA]` → WhatsApp

---

### 12. FAQ
**Objetivo:** Eliminar últimas dúvidas

6-8 perguntas frequentes em formato accordion

---

## Elementos Extras

### Pop-up de Captura
- **Trigger:** 10-15 segundos após entrada OU exit intent
- **Oferta:** "Receba valores e datas das próximas turmas"
- **Campos:** Nome, Email, Telefone
- **Destino:** Google Sheets

### Botão WhatsApp Flutuante
- Canto inferior direito, sempre visível
- Mensagem pré-preenchida

---

## Prompts para Google Stitch

### Prompt 1: Hero
```
Crie uma hero section para landing page de escola de tatuagem:
- Estilo: Dark mode moderno com acentos em dourado/bronze
- Layout: Split screen - texto à esquerda, imagem de tatuador à direita
- Headline grande emocional + subheadline
- Botão CTA verde vibrante
- Background: gradiente escuro com texturas sutis de tinta
```

### Prompt 2: Social Proof
```
Design uma seção de prova social com 5 cards horizontais:
- Números grandes: "12 Anos", "+5.000 Alunos", "+5M Views", "+156K Seguidores", "7 Países"
- Fundo escuro (#1a1a1a), texto branco, acentos dourados (#C9A962)
- Ícones minimalistas ao lado de cada número
```

### Prompt 3: Depoimentos
```
Crie seção de depoimentos com 3 cards em carrossel:
- Foto circular do aluno, nome, profissão anterior, citação, resultado atual
- Cards escuros com borda dourada sutil
- Aspas decorativas grandes
```

### Prompt 4: Página Completa Mobile
```
Landing page mobile-first para escola de tatuagem:
- Dark mode (#0d0d0d), acentos dourado (#D4AF37) e verde (#22C55E)
- Seções: Hero, números, método em 4 steps, depoimentos, galeria, investimento, FAQ, CTA final
- Botão WhatsApp flutuante
- Tipografia bold impactante nos headlines
```

---

## Checklist de Verificação

- [ ] Todos os CTAs redirecionam para WhatsApp correto
- [ ] Pop-up envia dados para Google Sheets
- [ ] Responsivo em mobile, tablet e desktop
- [ ] Core Web Vitals ok (Lighthouse)
- [ ] Meta tags e SEO configurados
- [ ] Imagens otimizadas
- [ ] Botão WhatsApp flutuante funcionando
