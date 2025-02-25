🌎 Mapeando Dados do IBGE com Folium: Visualização Dinâmica de Setores Censitários! 📊🗺️

Nos últimos dias, trabalhei para coletar dados do IBGE por setor censitário para o projeto Water mAIsure. O intuito é estudar as relações de variáveis socioeconômicas com a fraude de água. 

Como recorte dessa task construí de um mapa interativo utilizando Folium e GeoPandas para visualizar diferentes variáveis do IBGE em nível de setor censitário.

O que eu fiz?
- Carreguei um shapefile com a geometria dos setores censitários.
- Integrei dados do IBGE para adicionar variáveis socioeconômicas.
- Criei um mapa interativo onde o usuário pode selecionar a variável de interesse e visualizar sua distribuição espacial.

Principais desafios:
- Garantir que os dados geográficos estivessem no formato correto (WGS 84 - EPSG:4326).
- Tratar variáveis para evitar erros na escala de cores (dados ausentes e valores não numéricos).
- Incorporar um menu interativo para facilitar a alternância entre diferentes variáveis.

Esse tipo de ferramenta facilita a análise espacial de indicadores sociais e econômicos, tornando as informações mais acessíveis e compreensíveis para pesquisadores, gestores públicos e a sociedade em geral.
Se você trabalha com dados espaciais, econometria ou ciência de dados, essa abordagem pode ser muito útil para transformar grandes bases de dados em insights visuais poderosos! 

Com esse recorte, consegui entender mais sobre dados geoespaciais e bibliotecas fundamentais dessa área no Python: Folium e Geopandas.

No vídeo eu dou foco pra cidade de Cuiabá em Mato Grosso, cidade no qual estava analisando os dados. Como exemplo, ploto as variáveis V002 e V003 da tabela DomicílioRenda, no qual representam, respectivamente, o total do rendimento nominal mensal dos domicílios particulares e o total do rendimento nominal mensal dos domicílios particulares permanentes. 

# Como implementar? 

1 - Você deve baixar os arquivos shp do estado que você quer analisar no site do IBGE: https://www.ibge.gov.br/geociencias/organizacao-do-territorio/malhas-territoriais/26565-malhas-de-setores-censitarios-divisoes-intramunicipais.html
2 - Você deve baixar as variáveis socioeconômicas do censo no site do IBGE (por setor censitário): https://www.ibge.gov.br/estatisticas/sociais/trabalho/9662-censo-demografico-2010.html?edicao=10410

Extraia os arquivos no seu diretório e execute o código! Lembre-se de mudar o diretório!
