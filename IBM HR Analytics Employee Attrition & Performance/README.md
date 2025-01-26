# Análise Exploratória de Dados: IBM HR Analytics
*(Ainda em desenvolvimento)*

## Introdução e Objetivos
Este projeto tem como foco a análise exploratória de dados (EDA) utilizando o conjunto de dados fictício **IBM HR Analytics Employee Attrition & Performance**, disponível no [Kaggle](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset/data). O objetivo é identificar padrões e insights relacionados ao atrito de funcionários, explorando como aspectos demográficos, educacionais, organizacionais e de satisfação influenciam a retenção de talentos em uma organização fictícia.

O termo *attrition* (atrito)refere-se à redução gradual do número de funcionários devido a saídas naturais, como aposentadorias e demissões voluntárias, **geralmente sem reposição**. Por outro lado, *turnover* (rotatividade) engloba todas as saídas, voluntárias ou involuntárias, e **normalmente envolve reposições**. Compreender essa distinção é essencial para planejar estratégias eficazes de gestão de pessoas.

---

## Metodologia
A análise foi conduzida em etapas estruturadas, iniciando com a preparação e limpeza dos dados. Bibliotecas como `pandas` foram utilizadas para carregar o dataset, verificar valores nulos, identificar duplicatas e remover variáveis irrelevantes, como aquelas com valores constantes. A categorização das variáveis foi realizada para facilitar a análise, agrupando-as em categorias nominais, ordinais e quantitativas.

Foi aplicada a técnica do intervalo interquartil (IQR) para identificar *outliers* em variáveis numéricas. Além disso, otimizamos a memória convertendo variáveis categóricas para o tipo `category`, garantindo maior eficiência no processamento. 

---

## Características do Dataset
O conjunto de dados contém 1470 registros que descrevem informações sobre funcionários de uma organização fictícia, incluindo:
- Dados demográficos, como idade, gênero e estado civil;
- Informações profissionais, como cargo, departamento e tempo na empresa;
- Indicadores de satisfação e desempenho no trabalho;
- Formação educacional e áreas de especialização.

Após limpeza, o dataset foi considerado de alta qualidade, sem valores nulos ou duplicados, e com quatro variáveis removidas por serem constantes ou analiticamente irrelevantes.

---

## Resultados e Análises

Os resultados da análise exploratória revelaram diversos padrões importantes:

Os funcionários concentram-se majoritariamente na faixa etária de 31 a 36 anos, com uma distribuição de gênero de 60% homens e 40% mulheres. Quanto ao estado civil, a maior parte dos funcionários é casada (45,78%), seguida por solteiros (31,97%) e divorciados (22,24%). Em relação à formação educacional, 38,91% possuem graduação, enquanto 27,07% têm mestrado, com predomínio das áreas de Ciências Biológicas (Life Sciences) e Medicina (Medical).

No aspecto organizacional, o departamento de Pesquisa e Desenvolvimento (R&D) representa a maior parte da força de trabalho, com 961 funcionários, seguido pelo departamento de Vendas (446) e Recursos Humanos (63). Os níveis de satisfação geral com o ambiente e o trabalho são moderados, sugerindo espaço para melhorias.

---

## Recomendações e Interpretações

A análise revelou oportunidades importantes para a organização. A predominância masculina sugere a necessidade de estratégias para aumentar a diversidade de gênero, enquanto a concentração em áreas específicas de formação pode ser um indicativo de falta de diversificação educacional. Níveis moderados de satisfação no trabalho destacam a necessidade de ações voltadas à melhoria do ambiente organizacional e engajamento dos funcionários.

Além disso, o alto nível educacional dos funcionários indica um grande potencial para programas de desenvolvimento profissional, como mentoria e progressão de carreira. A diversificação das oportunidades de crescimento pode contribuir para maior retenção e engajamento.

---

## Próximos Passos

Com base nas descobertas da análise exploratória, o próximo passo será a implementação de algoritmos de **Machine Learning** para prever a rotatividade de funcionários e identificar os fatores mais influentes no atrito. Este processo incluirá:
- Pré-processamento dos dados para adequação aos modelos;
- Treinamento de algoritmos como regressão logística, árvores de decisão e random forest;
- Avaliação dos modelos com métricas como acurácia, precisão, recall e F1-score;
- Geração de recomendações práticas baseadas nos resultados.

O projeto estabelece uma base sólida para a tomada de decisões estratégicas, com potencial para melhorar significativamente a retenção de talentos e a gestão organizacional.
