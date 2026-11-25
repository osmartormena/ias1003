# Fundamentos de Modelagem e Análise de Dados

**Curso:** Tecnologia de Inteligência Artificial e Sistemas Autônomos (1º período)  
**Linguagem:** Python (Jupyter/Colab, NumPy, pandas, Matplotlib)

> **Premissas deste plano:** 15 semanas. Todos os dados são **simulados**; a semana 15 prevê, se disponível, o uso de dados reais de bancada.

---

## 1. Resultados de aprendizagem (proposta)

| RA | Descrição |
|----|-----------|
| RA1 | Organizar bases de dados, mobilizando ferramentas computacionais para extração de informações. |
| RA2 | Descrever variáveis via gráficos, mobilizando a modelagem de dados para apoio técnico. |
| RA3 | Estimar erro e incerteza de medições, mobilizando o raciocínio quantitativo para avaliar a confiabilidade de sensores. |
| RA4 | Resolver sistemas lineares com matrizes, mobilizando o cálculo computacional para modelar problemas de circuitos e de ajuste de dados. |
| RA5 | Ajustar e interpretar um modelo de tendência linear, mobilizando a análise de correlação para prever comportamentos. |
| RA6 | Preparar registros (logs) para análise, mobilizando técnicas de limpeza para alimentar modelos. |

---

## 2. Visão geral das 15 semanas

| Sem. | Tema | Bloco |
|:---:|------|-------|
| 1 | Do fenômeno ao dado; Python I | Python mínimo |
| 2 | Python II: laços, condicionais e funções | Python mínimo |
| 3 | Python III: NumPy, pandas e Matplotlib | Python mínimo |
| 4 | Álgebra linear I: vetores e matrizes | Álgebra linear |
| 5 | Álgebra linear II: sistemas lineares | Álgebra linear |
| 6 | Grandezas físicas, SI e sensores | Medição |
| 7 | Erro, incerteza e ruído · **Avaliação 1** | Medição |
| 8 | Estatística descritiva I | Estatística |
| 9 | Estatística descritiva II: distribuições e outliers | Estatística |
| 10 | Correlação | Modelagem |
| 11 | Regressão linear I: mínimos quadrados | Modelagem |
| 12 | Regressão linear II: qualidade do ajuste · **Avaliação 2** | Modelagem |
| 13 | Logs e persistência de dados | Preparação de dados |
| 14 | Limpeza, séries temporais e preparação para modelos | Preparação de dados |
| 15 | Projeto integrador: apresentações e devolutiva | Integração |

---

## 3. Planejamento semanal

### Semana 1 — Do fenômeno ao dado · Python I
- **Objetivo:** compreender como um fenômeno físico vira informação digital e executar os primeiros códigos em Python.
- **Teoria (1 h):** apresentação da disciplina, do plano e da avaliação; ciclo fenômeno → sensor → sinal → dado → informação; exemplos de sistemas autônomos.
- **Prática (2 h):** configuração do ambiente (Colab ou Jupyter); variáveis, tipos (`int`, `float`, `str`, `bool`), operações, `print` e `input`; primeiro notebook.
- **EaD (1 h):** questionário de diagnóstico (conhecimento prévio de programação e matemática) e lista de exercícios 1.
- **Integração:** combinar com *Programação para Sistemas Autônomos* quais tópicos de Python ficam com cada disciplina.

### Semana 2 — Python II: laços, condicionais e funções
- **Objetivo:** escrever pequenos programas com decisão, repetição e funções.
- **Teoria (1 h):** fluxo de controle e funções; leitura de código e depuração de erros comuns.
- **Prática (2 h):** `if/else`, `for`, `while`, listas e dicionários; funções com parâmetros e retorno; exercício: conversão de unidades e leitura de uma lista de medidas.
- **EaD (1 h):** lista de exercícios 2 (depuração de código com erros propostos).

### Semana 3 — Python III: NumPy, pandas e Matplotlib
- **Objetivo:** manipular vetores e tabelas e produzir gráficos simples.
- **Teoria (1 h):** por que usar vetores (vetorização); anatomia de um `DataFrame`; boas práticas de gráfico (eixos, unidades, legendas).
- **Prática (2 h):** `numpy.array`, operações vetorizadas; `pandas.DataFrame` criado a partir de dados simulados; gráficos de linha e dispersão com Matplotlib.
- **EaD (1 h):** lista de exercícios 3 — reproduzir um gráfico a partir de especificação.
- **Entrega:** notebook 1 (Python mínimo).

### Semana 4 — Álgebra linear I: vetores e matrizes
- **Objetivo:** representar dados e relações lineares por vetores e matrizes.
- **Teoria (1 h):** vetores, matrizes, soma, produto por escalar, produto matricial, transposta, identidade e inversa (ideia geométrica e numérica).
- **Prática (2 h):** operações com `numpy` (`@`, `.T`, `np.linalg.inv`); interpretar uma tabela de dados como matriz (linhas = amostras, colunas = variáveis).
- **EaD (1 h):** lista de exercícios 4.

### Semana 5 — Álgebra linear II: sistemas lineares
- **Objetivo:** resolver sistemas de 2 a 4 equações e interpretar o resultado.
- **Teoria (1 h):** sistema linear na forma matricial `Ax = b`; existência e unicidade de solução; condicionamento (noção).
- **Prática (2 h):** `np.linalg.solve`; modelar com matrizes o problema de malhas de um circuito CC com valores simulados e verificar a solução com a lei de Kirchhoff.
- **EaD (1 h):** problemas de sistemas lineares com contextos variados (misturas, circuitos, balanceamento).
- **Integração:** *Fundamentos de Eletricidade e Eletrônica* usa análise de malhas; avisar o(a) colega que esta semana é a oportunidade de combinar exemplos. Se o colega precisar antes, antecipar as semanas 4 e 5 para depois da semana 1.

### Semana 6 — Grandezas físicas, SI e sensores
- **Objetivo:** identificar grandezas, unidades e a forma como sensores geram dados.
- **Teoria (1 h):** grandezas e Sistema Internacional; algarismos significativos; resolução, faixa e sensibilidade de um sensor; representação numérica (ponto fixo e flutuante, noção).
- **Prática (2 h):** simular um sensor (por exemplo, temperatura) com resolução finita e quantização; efeito de truncar e arredondar leituras.
- **EaD (1 h):** estudo de um datasheet de sensor e preenchimento de um roteiro (faixa, resolução, precisão).
- **Integração:** *Sistemas Digitais* trata de ponto flutuante e erros de arredondamento; alinhar vocabulário (erro absoluto, erro relativo).

### Semana 7 — Erro, incerteza e ruído · Avaliação 1
- **Objetivo:** quantificar a incerteza de uma medição e distinguir ruído de sinal.
- **Teoria (1 h):** erro absoluto e relativo; incerteza do tipo A (média e desvio da média); ruído aleatório e erro sistemático; propagação simples de incerteza.
- **Prática (2 h):** simular N medidas de uma mesma grandeza com ruído gaussiano; calcular média, desvio-padrão e incerteza; ver como a incerteza cai com o aumento de N. Parte da aula reservada à **Avaliação 1**.
- **EaD (1 h):** conclusão e envio do notebook da Avaliação 1.
- **Avaliação 1 (prática, individual):** notebook com Python, álgebra linear e medição (semanas 1 a 7).

### Semana 8 — Estatística descritiva I
- **Objetivo:** resumir um conjunto de dados com medidas de posição e dispersão.
- **Teoria (1 h):** média, mediana, moda, amplitude, variância, desvio-padrão, coeficiente de variação; quando usar cada uma.
- **Prática (2 h):** `describe()` do pandas; histogramas; comparar duas séries simuladas de sensores (um preciso e outro ruidoso).
- **EaD (1 h):** lista de exercícios 5 com interpretação de resumos estatísticos.

### Semana 9 — Estatística descritiva II: distribuições e outliers
- **Objetivo:** reconhecer distribuições comuns e detectar valores atípicos.
- **Teoria (1 h):** distribuição normal e uniforme (noção); quartis e intervalo interquartil; critério do boxplot; outlier como erro ou como evento.
- **Prática (2 h):** gerar dados com `numpy.random`; histogramas, boxplots e gráficos de densidade; inserir falhas simuladas e detectá-las.
- **EaD (1 h):** ficha de interpretação de gráficos (quais conclusões são justificáveis).
- **Integração:** preparar a base propositalmente desbalanceada que *Ética, Sustentabilidade e Humanização da Tecnologia* poderá usar para discutir vieses.

### Semana 10 — Correlação
- **Objetivo:** medir e interpretar a relação entre duas variáveis.
- **Teoria (1 h):** covariância; coeficiente de correlação de Pearson; correlação não implica causalidade.
- **Prática (2 h):** gráficos de dispersão, `corr()` e mapa de calor de correlações; exemplos com correlações espúrias.
- **EaD (1 h):** lista de exercícios 6 — classificar correlações em gráficos fornecidos.

### Semana 11 — Regressão linear I: mínimos quadrados
- **Objetivo:** ajustar uma reta a dados e compreender o critério de mínimos quadrados.
- **Teoria (1 h):** modelo `y = a·x + b`; minimizar a soma dos quadrados dos resíduos; equações normais em forma matricial (conecta as semanas 4 e 5).
- **Prática (2 h):** ajustar uma reta de três formas: com as equações normais em `numpy`, com `np.polyfit` e com `scipy.stats.linregress` ou `scikit-learn`; comparar os resultados.
- **EaD (1 h):** lista de exercícios 7.
- **Integração:** exemplo com tensão e corrente simuladas (lei de Ohm) estimando a resistência com sua incerteza.

### Semana 12 — Regressão linear II: qualidade do ajuste · Avaliação 2
- **Objetivo:** avaliar um ajuste e usá-lo para prever.
- **Teoria (1 h):** resíduos, R², erro quadrático médio; extrapolar × interpolar; limites do modelo linear.
- **Prática (2 h):** gráfico de resíduos; separar dados de ajuste e de teste; prever um valor novo com intervalo de plausibilidade. Parte da aula reservada à **Avaliação 2**.
- **EaD (1 h):** conclusão e envio do notebook da Avaliação 2.
- **Avaliação 2 (prática, individual):** estatística descritiva, correlação e regressão (semanas 8 a 12).

### Semana 13 — Logs e persistência de dados
- **Objetivo:** ler, inspecionar e armazenar registros de sistemas.
- **Teoria (1 h):** o que é um log; formatos CSV, JSON e texto; estrutura de uma base de dados e identificação de campos (inclusive dados pessoais, que serão discutidos em *Ética*).
- **Prática (2 h):** `read_csv`, `read_json`, `to_csv`; inspeção com `info()` e `head()`; leitura de um log de eventos simulado (timestamps, níveis, mensagens).
- **EaD (1 h):** lista de exercícios 8 — descrever a estrutura de três bases fornecidas.

### Semana 14 — Limpeza, séries temporais e preparação para modelos
- **Objetivo:** transformar um log bruto em uma base pronta para análise.
- **Teoria (1 h):** valores ausentes, duplicados e inconsistentes; tratamento (remover, imputar); normalização (noção); série temporal e reamostragem; separar entradas e saída de um modelo.
- **Prática (2 h):** `isna()`, `dropna()`, `fillna()`, `to_datetime()`, `resample()`, médias móveis; limpar um log com falhas de leitura simuladas e plotar o resultado.
- **EaD (1 h):** preparação do mini-projeto: escolha do tema e do conjunto de dados.
- **Integração:** o log com tendência e anomalias pode ser o do caso de manutenção preditiva de *Fábricas Inteligentes e Fundamentos de Autonomia*.

### Semana 15 — Projeto integrador: apresentações e devolutiva
- **Objetivo:** executar o fluxo completo, do dado bruto ao resultado interpretado, e comunicá-lo.
- **Teoria (1 h):** orientações finais para a apresentação; revisão dos conceitos centrais.
- **Prática (2 h):** apresentações curtas (5 a 8 min por grupo) e discussão.
- **EaD (1 h):** envio do relatório/notebook final e autoavaliação.
- **Entrega:** notebook do mini-projeto com problema, dados, limpeza, análise descritiva, ajuste linear, conclusões e limitações. **Se houver dados reais de bancada ao final do semestre, usá-los como estudo de caso comparativo.**

---

## 4. Avaliação (proposta de pesos)

| Instrumento | Peso |
|-------------|:----:|
| Atividades EaD e listas de exercícios (semanas 1 a 14) | 20% |
| Avaliação 1: prática individual (semana 7) | 20% |
| Avaliação 2: prática individual (semana 12) | 25% |
| Mini-projeto integrador (semana 15) | 35% |

Sugestão: avaliar o **raciocínio**, não apenas o código. Em cada avaliação, incluir uma questão em que o aluno explique, por escrito, por que escolheu determinado método e o que o resultado significa.

---

## 5. Pontos de integração com as demais disciplinas

| Disciplina | Ponto de contato | Semana |
|------------|------------------|:------:|
| Programação para Sistemas Autônomos | Divisão do conteúdo de Python; padrão de comentários e versionamento | 1–3 |
| Fundamentos de Eletricidade e Eletrônica | Sistemas lineares (malhas); incerteza de medição; ajuste da lei de Ohm | 5, 7, 11 |
| Sistemas Digitais | Vocabulário de erro numérico, arredondamento e ponto flutuante | 6 |
| Fábricas Inteligentes e Fundamentos de Autonomia | Log de vibração/temperatura para manutenção preditiva | 14–15 |
| Ética, Sustentabilidade e Humanização da Tecnologia | Base desbalanceada para viés; dados pessoais em logs; custo computacional | 9, 13, 15 |

---

## 6. Pontos a combinar com os colegas
1. **Python primeiro:** confirmar que *Programação* abordará Python (variáveis, laços, funções) nas primeiras semanas e deixará C para depois.
2. **Sistemas lineares:** saber em que semana *Eletricidade* precisará de análise de malhas.
3. **Vocabulário de erro e incerteza:** definir uma única notação para as três disciplinas.
4. **Política de IA em código (vibe coding):** acordar uma regra comum sobre o uso de assistentes de código e como declarar esse uso.
5. **Modelo único de relatório:** um padrão de documento para os trabalhos de todas as disciplinas.
6. **Dados de bancada:** definir se algum conjunto real será compartilhado no fim do semestre.

---

## 7. Ajustes possíveis
- **Menos de 15 semanas:** fundir as semanas 8 e 9 (estatística) e as semanas 13 e 14 (logs), e reduzir o tempo de prática nas semanas 2 e 3.
- **Alunos com pouca base em Python:** estender a semana 3 em mais uma aula e comprimir a semana 6.
- **Eletricidade precisa de sistemas lineares cedo:** trocar a ordem para Python (1 a 3), álgebra linear (4 e 5) logo no início, o que já está previsto; se for ainda antes, antecipar a semana 5 para a semana 3.
- **Sem aula em laboratório de informática:** usar Google Colab, que dispensa instalação, e manter as listas EaD como reforço.
