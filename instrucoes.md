# 📝 Instruções da Prova Técnica

Obrigado por participar do processo seletivo para a Vaga de Analista Jr. de Middle Office da ATMO ENERGIA! 
Abaixo estão as instruções detalhadas para a realização da prova técnica.

---

## 📂 Dataset

Você encontrará os arquivos `vazoes.csv` e `posto.csv` na pasta `dados/`. Use estes dados para responder às questões abaixo.

---

## 🧪 Tarefas

### 1. Leitura e entendimento dos dois arquivos
- Carregue o dado `vazoes.csv` com `pandas`
- Exiba as primeiras linhas e descreva brevemente o que você entendeu sobre os dados
- Carregue o dado `posto.csv` com `pandas`
- Exiba as primeiras linhas e descreva brevemente o que você entendeu sobre os dados
- Existe alguma relação entre eles? Há alguma chave ou campo comum? 
- Qual arquivo você classificaria como cadastro/dimensão (dados de referência)?
- E qual arquivo são de fato/evento (ocorrência ao longo do tempo)?

### 2. Limpeza e pré-processamento
- Verifique se há valores ausentes ou inconsistentes nos dois arquivos (vazoes.csv e posto.csv)
- Trate os dados de forma apropriada:
- Preencha, remova ou justifique o tratamento dos valores ausentes
- Corrija tipos de dados quando necessário (ex: colunas que deveriam ser datetime ou float)
- Verifique se há dados fora do domínio esperado
    Dica: Vazão é uma medida física (m³/s) e não faz sentido ser negativa
- Comente brevemente quais decisões você tomou e por quê

### 3. Análise Estatística Descritiva
- Apresente estatísticas descritivas dos dados de vazão:
    . Média, mediana, desvio-padrão, valores mínimos e máximos, percentis, etc.
- Explore possíveis correlações entre variáveis disponíveis nos dados
    . Exemplo: relação entre submercados, bacias ou entre postos vizinhos
- Crie ao menos 2 gráficos que ajudem a entender o comportamento das vazões ao longo do tempo
    Dicas: Use histogramas, boxplots, heatmaps de correlação, linhas de tendência ou gráficos de série temporal
    Use matplotlib, seaborn, ou a biblioteca de sua preferência

### 4. Análise Exploratória 
- É possível agrupar os dados? De quantas maneiras?
    . Pense em agrupamentos temporais (por exemplo: mês, ano, estação do ano)
    . Pense em agrupamentos por atributos do posto, como:
        . Submercado
        . Bacia hidrográfica
        . Tipo do posto (se existir)
- Explore os diferentes tipos de agrupamentos possíveis
- Gere um ou mais dataframes com esses agrupamentos
- Utilize groupby, agg, ou outras funções que achar necessário
- Comente sobre o raciocínio adotado:
    . Por que escolheu esses agrupamentos?
    . Qual informação interessante pode ser extraída deles?

### 5. Modelo de Regressão 
- Escolha duas variáveis do conjunto de dados de vazoes.csv:
    . Uma como variável independente (explicativa)
    . Outra como variável dependente (a ser estimada)
- Aplique uma regressão linear simples ou outro modelo básico de regressão
    . Você pode usar scikit-learn, statsmodels ou outro pacote que preferir
- Avalie e comente os resultados:
    . O modelo faz sentido?
    . Os resíduos (erros) estão bem distribuídos?
    . O R² ou outros indicadores são bons?
- Gere ao menos 1 gráfico de previsão vs. real ou resíduos para ilustrar a performance

---

## 🧠 Dicas

- Utilize células de texto para explicar seu raciocínio
- Prefira gráficos limpos e informativos
- Seu código deve ser funcional e replicável
- Evite usar bibliotecas que não sejam mencionadas, a menos que justifique

---

## ✅ Entrega

Finalize todas as respostas no arquivo `respostas.ipynb`.

---

Boa sorte! Qualquer dúvida, entre em contato com o responsável pela prova.
