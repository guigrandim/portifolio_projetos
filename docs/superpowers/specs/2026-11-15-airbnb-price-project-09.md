# Airbnb Price como projeto 09

## Objetivo

Adicionar ao portfólio o projeto Airbnb Price de Amsterdam como projeto 09, usando a imagem local e o padrão dos cases existentes. O destaque comercial deve mostrar o impacto econômico projetado sem tratá-lo como retorno realizado.

## Conteúdo aprovado

- Usar `images/projeto09.png` no card.
- Título: “Airbnb Price compara a diária anunciada com a estimativa do modelo.”
- Resumo: “Criei um simulador que estima a diária em Amsterdam com base no bairro e nas características do imóvel. Ele também mostra a diferença para o preço anunciado.”
- Resultado em destaque: “Volume bruto de reservas projetado: +€ 2,05 milhões ao ano (+1,75%).”
- Contexto do resultado: “Na simulação com 20.026 anúncios da base de dezembro de 2018, trocar os preços anunciados pelas referências do modelo levou o volume bruto anual de € 117,22 milhões para € 119,27 milhões. A conta mantém o número estimado de noites. É uma projeção, não um resultado realizado. Para calcular o ROI percentual, faltam dados sobre a receita adicional da plataforma e os custos do projeto.”
- Métricas do modelo: “No teste histórico com 3.005 anúncios, o LightGBM teve MAPE de 25,98% e erro absoluto médio (MAE) de € 38,95 por noite.”
- Stack: Python, pandas, NumPy, SciPy, scikit-learn, Boruta, XGBoost, LightGBM, Optuna, Streamlit, Altair, JupyterLab, Git e GitHub.
- Links: repositório `https://github.com/guigrandim/airbnb_price` e aplicativo `https://airbnbprice.streamlit.app/`.

## Implementação

Adicionar o card ao fim da lista atual de cases em `index.html`, com o marcador 09, seguindo a estrutura `.case-study` existente. Preservar o estilo atual e não introduzir dependências nem alterar CSS ou JavaScript.
