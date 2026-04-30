## Sobre esta pesquisa
Esta pesquisa investiga como empresas reais implementam (ou ignoram) acessibilidade digital em sites e apps, focando obrigações legais, casos reais e práticas de líderes tech.

## O que descobrimos (Principais Achados)
- PicPay e Banco Original (Grupo J&F) não possuem páginas dedicadas a acessibilidade em seus sites principais ou centros de ajuda, ignorando visibilidade sobre conformidade com WCAG ou LBI. Entretanto, O Picpay investe em acessibildade digital por meio de biometria facial e digital para autenticação segura, além de IA para interpretar áudios e imagens no PIX via WhatsApp. [Clique aqui para acessar a fonte.](https://www.reclameaqui.com.br/picpay/falta-de-acessibilidade-descaso_yyislrjme9b-_k30/)
- A Magazine Luiza tem uma página dedicada a acessibilidade em seu site, listando contatos como 0800 773 3838 e destacando esforços de inclusão, o que sugere proatividade em vez de violações. [Acessibilidade Magazine Luiza](https://especiais.magazineluiza.com.br/acessibilidade/)
- Domino's Pizza nos EUA enfrenta um processo desde 2016 por site inacessível a deficientes visuais, chegando à Suprema Corte; no Brasil, não há multas específicas por sites, mas MPF cobra regulamentação urgente da LBI art. 63. [Dominios quer prova na suprema corte dos eua que sites não precisam ser acessiveis a deficientes visuais](https://www.b9.com.br/112162/dominos-quer-provar-na-suprema-corte-dos-eua-que-sites-nao-precisam-ser-acessiveis-a-deficientes-visuais/) e [Falta de acessibilidade nos sites e tema de ação do ministeria publico federal](https://mwpt.com.br/falta-de-acessibilidade-nos-sites-e-tema-de-acao-do-ministerio-publico-federal/)
- Líderes como Microsoft, Apple e Google integram acessibilidade via WCAG 2.1/2.2, EN 301 549 e Section 508, com relatórios de conformidade, features como Lupa e Nutrition Labels, e design inclusivo desde o início. [Microsoft](https://www.microsoft.com/pt-br/accessibility), [Fórum da Apple sobre acessibilidade em seus produtos](https://developer.apple.com/forums/tags/accessibility), [Artigo sobre acessibilidade digital](https://web.dev/articles/a11y-tips-for-web-dev?hl=pt-br) e [Apple Acessibilidade](https://www.apple.com/accessibility/)

## Casos
 A seção principal com o produto obrigatório da sua dimensão.
 (relatório, mapa comparativo ou infográfico — em formato Markdown ou imagem)

## Como isso afeta o nosso trabalho como desenvolvedores
A falta de acessibilidade digital em empresas brasileiras cria riscos legais crescentes, multitarefas para devs (testes manuais + automação) e pressão por conformidade com a legislação, impactando prazos e qualidade do código.

Como solucionadores, podemos incluir acessibilidade desde o design, usando ferramentas como Lighthouse ou WAVE para análises automáticos. Exemplo: adicione alt descritivo em imagens: 
```html
(<img src="logo.png" alt="Logo do PicPay">)`
```

Adote políticas de empresa: realize análises regulares (ex.: Microsoft Accessibility Insights) e inclua testes manuais com leitores de tela nos processos de CI/CD.

**Risco pessoal para nós desenvolvedores:** Desenvolvedores podem ser responsabilizados em processos se ignorarem alt, ARIA ou keyboard navigation.

### Práticas concretas

```html
<!-- ANTES: Imagem sem contexto -->
<img src="produto.jpg">

<!-- DEPOIS: WCAG 1.1.1 -->
<img src="produto.jpg" alt="Smartphone Samsung Galaxy S24, 128GB, preto">

<!-- Keyboard focus visível -->
button:focus-visible { 
  outline: 2px solid #0066cc; 
  outline-offset: 2px; 
}
```

## Referências
- Ministério Público Federal. Nova cobrança do MPF alerta empresas que não priorizam acessibilidade digital. 2025. https://diariopcd.com.br/nova-cobranca-do-mpf-alerta-empresas-que-nao-priorizam-acessibilidade-digital/
- Governo Federal do Brasil. Guia de Boas Práticas para Acessibilidade Digital. 2023. https://www.gov.br/governodigital/pt-br/acessibilidade-e-usuario/acessibilidade-digital/guiaboaspraaticasparaacessibilidadedigital.pdf
- Web para Todos (wpt). Falta de acessibilidade nos sites e tema da ação do ministério público federal. 2018. https://mwpt.com.br/falta-de-acessibilidade-nos-sites-e-tema-de-acao-do-ministerio-publico-federal/
- B9. Domino’s quer provar na Suprema Corte dos EUA que sites não precisam ser acessíveis a deficientes visuais. 2019. https://www.b9.com.br/112162/dominos-quer-provar-na-suprema-corte-dos-eua-que-sites-nao-precisam-ser-acessiveis-a-deficientes-visuais/
- Diário PCD. Nova cobrança do MPF alerta empresas que não priorizam acessibilidade digital. 2025. https://diariopcd.com.br/nova-cobranca-do-mpf-alerta-empresas-que-nao-priorizam-acessibilidade-digital/