# Contexto do Projeto - Projeto Tattoo

## O que é este projeto
Landing page de alta conversão para **Escola de Tatuagem Projeto Tattoo** - curso presencial de 40h que ensina pessoas do zero a tatuar em 1 mês.

## Público-alvo
Pessoas que querem começar a tatuar ou estão iniciando, buscando transformação de carreira e liberdade financeira através da arte.

## Stack
- **Astro 5.x** (framework estático)
- **CSS puro** com variáveis
- **Fontes:** Bebas Neue + Outfit (Google Fonts)
- **Paleta:** Dark (#0a0a0a), Gold (#C9A962), Green (#22C55E)

## Estrutura de arquivos importantes
```
/src
  /components
    Hero.astro          # Seção inicial emocional
    PainPoints.astro    # Dores do público
    Transformation.astro # Solução
    SocialProof.astro   # Números (12 anos, 5000 alunos)
    Method.astro        # Timeline 4 semanas
    Testimonials.astro  # Depoimentos
    Portfolio.astro     # Galeria trabalhos
    Investment.astro    # Potencial de ganhos
    Included.astro      # O que está incluso
    Objections.astro    # Quebra objeções
    FAQ.astro           # Perguntas frequentes
    FinalCTA.astro      # CTA urgência
    WhatsAppButton.astro # Botão flutuante
    PopupForm.astro     # Pop-up captura leads
  /layouts
    Layout.astro        # Layout base com CSS global
  /pages
    index.astro         # Página principal
/PLANO.md               # Plano completo com copy e status
```

## Comandos
```bash
npm run dev     # Inicia servidor → http://localhost:4321
npm run build   # Build para produção
```

## O que falta configurar
1. Número real do WhatsApp (substituir 5511999999999)
2. URL do Google Apps Script para integração Sheets
3. Imagens reais (portfolio, depoimentos, hero)

## Decisões de negócio
- NÃO mostrar preço na página (revelar só no WhatsApp)
- Tom equilibrado: emotivo + prático
- Usar depoimentos existentes + coletar mais

## Análise da concorrência
A página foi inspirada na estrutura emocional da **The Void Tattoo**, mas com identidade visual própria (dark mode premium com gold/green).

## Copy principal
- **Hero:** "Você sente que nasceu pra viver de arte, mas está preso numa vida que não é sua?"
- **Dor:** "A cada domingo à noite, aquele aperto no peito volta..."
- **Transformação:** "E se eu te dissesse que em 30 dias você pode estar tatuando de verdade?"
- **CTA:** "Quero começar minha transformação"
