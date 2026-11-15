# Redesign do portfólio para atrair clientes de Analytics

## Intenção

Transformar o portfólio atual em uma apresentação comercial clara para potenciais clientes, mostrando a experiência de Guilherme em Data Science e Analytics por meio de problemas de negócio, métodos e resultados verificáveis. Em poucos segundos, a pessoa deve entender como ele pode ajudar e como iniciar uma conversa.

## Objetivos e limites

- Explicar a oferta em linguagem de negócio: analytics e BI, modelagem preditiva e soluções de dados de ponta a ponta.
- Dar destaque a estudos de caso reais, com contexto, abordagem e resultado, sem inventar métricas nem sugerir causalidade não demonstrada.
- Mostrar credenciais e experiência sem deixar a longa lista de ferramentas dominar a página.
- Tornar email e WhatsApp fáceis de encontrar e usar.
- Manter o site estático em HTML, CSS e JavaScript, preservando os links atuais dos projetos e o suporte a GitHub Pages.
- Entregar o redesign executável neste repositório e usar a tela final do Stitch como referência visual; o Code Layer existente no Figma permanece como artefato de design.
- Não incluir formulários com backend, CMS, frameworks ou novas dependências de runtime.
- Usar a direção escura e técnica do Stitch com hierarquia clara, sem gráficos ou resultados inventados.

## Abordagens consideradas

1. **Consultoria orientada a decisões — escolhida.** Abre com uma proposta de valor e um convite para conversar; apresenta serviços e cases pela combinação problema, método e resultado. É a melhor correspondência ao objetivo de conquistar clientes, mantendo a prova técnica visível.
2. **Portfólio de pesquisa.** Coloca metodologia, ferramentas e detalhes dos modelos no centro. Demonstra profundidade, mas demora mais para explicar a oferta e chegar ao contato.
3. **Laboratório visual de dados.** Usa gráficos e linguagem de dashboard como identidade principal. Pode chamar atenção, mas corre o risco de parecer uma demonstração técnica em vez de uma oferta de analytics.

O usuário definiu o objetivo e deixou a direção visual em aberto; a primeira abordagem é a recomendação adotada, sujeita à aprovação deste documento.

## Público e ação principal

O público é formado por empresas e decisores que precisam entender melhor seus dados, acompanhar a operação ou prever resultados. A ação principal é iniciar uma conversa sobre um desafio de dados. A ação secundária é explorar um case completo ou seu repositório.

## Estrutura da página

1. **Abertura:** navegação curta; promessa em português que conecta dados a decisões de negócio; CTA para conversar e link para os cases. Um bloco visual original apresenta o fluxo API → base consolidada → projeção e uma métrica contextualizada do case de compras públicas. A métrica de R$ 492 milhões deve estar identificada como potencial estimado.
2. **Como posso ajudar:** três frentes compreensíveis para clientes: Analytics e BI; análise e modelagem preditiva; produtos e pipelines de dados. Ferramentas aparecem como apoio, não como títulos da oferta.
3. **Cases:** apresentar os sete projetos existentes: compras públicas, Rossmann, SRAG, mercado de games, cafeterias, Curry Company e ensaios de Machine Learning. Cada case mantém imagem, stack, links e resultado documentado. O valor de R$ 492 milhões é potencial estimado; os demais resultados são identificados como previsão, métrica técnica ou variação observada conforme a evidência disponível.
4. **Experiência e método:** formação na UNICAMP e USP, experiência em dados no esporte de alto rendimento e o processo de transformar uma pergunta em análise, solução e decisão. As habilidades são agrupadas por capacidade, sem repetir a lista extensa atual.
5. **Contato:** convite direto, email e WhatsApp, mantendo LinkedIn e GitHub como caminhos secundários.

## Direção visual

- **Paleta:** fundo `#0A0E14`, superfícies `#0E131A` e `#141922`, ciano `#22D3EE`, laranja `#F97316`, texto `#F1F5F9` e texto secundário `#94A3B8`, derivada do tema do Stitch.
- **Tipografia:** Space Grotesk para títulos e IBM Plex Sans para texto, com monoespaçada de sistema nos rótulos técnicos. Fontes locais evitam uma dependência externa em tempo de execução.
- **Layout:** navegação lateral fixa no desktop e barra compacta com navegação horizontal no celular; abertura em duas colunas com proposta comercial e painel do case de compras públicas; serviços, cases em grade, stacks agrupadas, experiência e contato.
- **Princípio de composição:** ciano sinaliza estrutura e informação técnica; laranja destaca CTAs e resultados de negócio. O destaque de ROI sempre informa se o número é potencial, previsto, observado ou não calculado.
- **Acessibilidade e movimento:** bom contraste, foco de teclado visível, navegação sem depender de animação e respeito a `prefers-reduced-motion`.

## Restrições de implementação

O repositório é um site estático do template Hyperspace. `index.html` contém conteúdo, navegação e metadados; `assets/css/custom.css` implementa localmente o sistema visual do Stitch. Não importar o Tailwind CDN, fontes remotas ou imagens geradas pelo HTML do Stitch: usar as fontes e imagens já disponíveis no repositório, preservando o funcionamento em GitHub Pages.

## Chamadas de implementação

O modelo visual foi gerado no Stitch e já está representado pelo Code Layer no Figma. Nesta implementação, preservar a promessa comercial, os sete cases, todas as stacks e as ressalvas existentes, em especial a limitação do classificador de SRAG. Não acrescentar ofertas nem alegações de ROI que os dados não sustentem.
