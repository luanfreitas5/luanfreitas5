<div align="center">
  <img src="banner/github-header-banner.png" alt="Luan Freitas - Cientista de Dados: Python, IA, NLP e Big Data" style="max-width: 50%;">
</div>

<h1 align="center">Luan Freitas</h1>

<p align="center">
  <strong>Cientista de Dados · Engenheiro de Inteligência Artificial</strong><br>
  Machine Learning aplicado, MLOps, NLP em português e IA Responsável<br>
  <sub>Bacharel em Ciência da Computação — Universidade de Brasília (UnB)</sub>
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/luanfreitas5/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="https://kaggle.com/luanfreitas5"><img src="https://img.shields.io/badge/Kaggle-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white" alt="Kaggle"></a>
  <a href="https://medium.com/luan.mgf"><img src="https://img.shields.io/badge/Medium-000000?style=for-the-badge&logo=medium&logoColor=white" alt="Medium"></a>
  <a href="https://stackoverflow.com/users/luan-freitas"><img src="https://img.shields.io/badge/Stack_Overflow-F58025?style=for-the-badge&logo=stackoverflow&logoColor=white" alt="Stack Overflow"></a>
  <a href="mailto:luan.mgf@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="E-mail"></a>
</p>

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=luanfreitas5&label=Visualiza%C3%A7%C3%B5es+do+perfil&color=0e75b6&style=flat-square" alt="Contador de visualizações do perfil" />
</p>

---

## 👋 Sobre mim

Construo **sistemas de machine learning que sobrevivem fora do notebook**: pipelines reprodutíveis,
contratos de dados validados, métricas honestas com intervalo de confiança e modelos servidos via API
ou dashboard. Meu foco está na interseção entre **rigor científico e engenharia de software**.

- 🔭 Trabalhando em um **portfólio de projetos ponta a ponta** em ML aplicado, MLOps e NLP em português
- 🌱 Aprofundando em **IA Generativa (LLMs locais e RAG)** e **Computação em Nuvem**
- 🧠 Interesses: **IA Responsável** — explicabilidade (SHAP), calibração de probabilidades e auditoria de fairness
- 👯 Aberto a colaborações em **saúde, finanças, educação e pesquisa aplicada**
- 💬 Pergunte-me sobre **ciência de dados, aprendizado de máquina e NLP em pt-BR**
- 📫 Contato: **luan.mgf@gmail.com** · [LinkedIn](https://www.linkedin.com/in/luanfreitas5/)

<div align="center">
  <img src="gif/Social Media Hello GIF by Jasper AI.gif" alt="Animação ilustrando um robô" height="180" loading="eager" />
</div>

---

## 🚀 Projetos em destaque

Cinco projetos ponta a ponta, cada um cobrindo um pilar diferente do ciclo de vida de ML —
de explicabilidade de negócio a MLOps de produção, fairness, benchmark científico e LLMs locais.

| Projeto | Problema | Diferencial técnico | Stack principal |
|---|---|---|---|
| **[🔮 Previsão de Churn Explicável](https://github.com/luanfreitas5/previsao-churn-explicavel)** | Identificar clientes com risco de não recomprar no marketplace Olist | SHAP traduzido para linguagem de negócio + auditoria de fairness por UF | `Polars` `LightGBM` `SHAP` `Fairlearn` `MLflow` `Streamlit` |
| **[🛡️ MLOps — Detecção de Fraude](https://github.com/luanfreitas5/mlops-deteccao-fraude)** | Fraude em ~284k transações com desbalanceamento extremo (~0,17%) | Ciclo MLOps completo: DVC + MLflow + API + CI/CD, com limiar sensível a custo | `XGBoost` `DVC` `MLflow` `FastAPI` `Docker` `GitHub Actions` |
| **[⚖️ Risco de Diabetes com Fairness](https://github.com/luanfreitas5/risco-diabetes-fairness)** | Triagem de risco de diabetes a partir do BRFSS 2015 (~253k respostas) | Calibração de probabilidade + auditoria de subgrupos + Model Card e Datasheet | `LightGBM` `Fairlearn` `SHAP` `Streamlit` `Plotly` |
| **[📊 Benchmark de Sentimento pt-BR](https://github.com/luanfreitas5/sentimento-ptbr-benchmark)** | BERTimbau realmente supera baselines clássicos? E generaliza entre domínios? | Avaliação *cross-dataset* N×N com gap de generalização e teste de McNemar | `BERTimbau` `Transformers` `scikit-learn` `MLflow` `uv` |
| **[🤖 Emoção em Tweets com LLM Local](https://github.com/luanfreitas5/tweets-emocao-llm-local)** | Emoção e tópicos em ~800k tweets em português | Arquitetura híbrida: Python calcula, LLM local **apenas** redige a explicação | `BERTopic` `Ollama` `Llama 3.1` `FastAPI` `Pydantic` |

<details>
<summary><b>📖 Ver detalhamento de cada projeto</b></summary>

<br>

### 🔮 [previsao-churn-explicavel](https://github.com/luanfreitas5/previsao-churn-explicavel) — Churn explicável no e-commerce brasileiro

**Problema de negócio.** No dataset público da Olist, a maioria dos clientes compra uma única vez.
Prever quem não voltará é um problema desbalanceado e com alto risco de vazamento temporal.

**Abordagem.** Features **RFM** (recência, frequência, valor) calculadas exclusivamente sobre o
histórico anterior ao *cutoff*, evitando vazamento por construção. Modelo **LightGBM** dentro de um
`Pipeline` do scikit-learn com balanceamento de classes.

**Rigor de avaliação.** Métrica principal **PR-AUC** (*Average Precision*) com **IC 95% via bootstrap**,
comparação contra baseline, análise de calibração (**Brier score**) e avaliação de fairness por estado
(UF) com `fairlearn`.

**Entrega.** Dashboard **Streamlit** que traduz os valores SHAP em explicações de negócio por cliente —
transformando score em decisão de retenção acionável.

---

### 🛡️ [mlops-deteccao-fraude](https://github.com/luanfreitas5/mlops-deteccao-fraude) — Ciclo MLOps completo

**Problema.** Detecção de fraude em ~284.000 transações anonimizadas (ULB Credit Card Fraud), com
apenas **~0,17% de casos positivos** — um cenário que expõe qualquer fragilidade de engenharia.

**Modelagem.** **XGBoost** com `scale_pos_weight`, baseline de Regressão Logística e SMOTE opcional
*dentro* do pipeline (nunca antes do split). Limiar de decisão escolhido por **custo assimétrico**
— falso negativo pesa muito mais que falso positivo — em vez do 0.5 padrão.

**Infraestrutura MLOps.**
- **DVC** para versionamento de dados e estágios reprodutíveis do pipeline
- **MLflow** registrando SHA do commit e hash do dataset em cada execução
- **FastAPI + Pydantic** validando schema na inferência, prevenindo *train-serve skew*
- **Pandera** como contrato de dados nas fronteiras do pipeline e da API
- **GitHub Actions** para lint, testes (≥80% de cobertura) e documentação
- **Docker Compose** orquestrando API e MLflow UI

**Métricas.** PR-AUC como métrica principal (não acurácia, não ROC-AUC), com **IC 95% por bootstrap**,
além de recall/precisão e Brier score para calibração.

---

### ⚖️ [risco-diabetes-fairness](https://github.com/luanfreitas5/risco-diabetes-fairness) — IA Responsável em triagem de saúde

**Problema.** Triagem de risco de diabetes a partir de fatores autorrelatados do inquérito
**BRFSS 2015** (~253k respostas, prevalência ~14%).

**Por que é diferente.** O objetivo não é maximizar acurácia — é entregar um modelo **auditável**:

- **Calibração** com `CalibratedClassifierCV`, para que a probabilidade signifique algo clinicamente
- **Limiar operacional de 0.30**, priorizando recall (o custo de um falso negativo em triagem é alto)
- **Auditoria de fairness** com `fairlearn` por `Sex`, `AgeBand`, `Income` e `Education`
- **Model Card e Datasheet** documentando escopo, limitações e uso pretendido

**Entrega.** Dashboard **Streamlit + Plotly** para exploração interativa e site de documentação MkDocs.

---

### 📊 [sentimento-ptbr-benchmark](https://github.com/luanfreitas5/sentimento-ptbr-benchmark) — Benchmark reprodutível em português

**Pergunta de pesquisa.** Fine-tuning de **BERTimbau** compensa frente a um baseline TF-IDF +
Regressão Logística? E o modelo **generaliza entre domínios**?

**Desenho experimental.** Cinco corpora rotulados em pt-BR (`b2w`, `buscape`, `olist`, `utlc_apps`,
`utlc_movies`). Cada modelo é treinado em um domínio e avaliado em **todos os cinco** — produzindo uma
**matriz cross-dataset N×N** que separa desempenho *in-domain* (diagonal) de *out-of-domain*.

**Rigor estatístico.** **F1-macro** com IC 95% por bootstrap, **gap de generalização**
(média in-domain − média out-of-domain) e **teste de McNemar** para significância entre baseline e
BERTimbau — porque uma diferença de pontos não é, por si só, uma diferença real.

**Reprodutibilidade.** Sementes fixas, lock files versionados, hashes SHA-256 dos corpora e CLI
padronizada (`uv run python -m src.main`).

---

### 🤖 [tweets-emocao-llm-local](https://github.com/luanfreitas5/tweets-emocao-llm-local) — LLM local com fronteira de responsabilidade

**Problema.** Análise de emoção e tópicos em **~800.000 tweets em português**, com explicações legíveis
por humanos.

**Decisão de arquitetura.** *"LLMs são ótimos escrevendo, e péssimos calculando."* A responsabilidade é
separada de forma estrita:

- **Python** faz limpeza, classificação de sentimento (**BERTimbau**), clusterização de tópicos
  (**BERTopic** + `sentence-transformers`) e cálculo de todas as métricas
- **LLM local** (`llama3.1:8b` via **Ollama**) recebe **apenas JSON já calculado** e redige o resumo

Isso elimina alucinação numérica por construção — o modelo nunca tem a chance de inventar um número —
e mantém todo o processamento em máquina local, sem enviar dados a APIs externas.

**Avaliação.** F1-macro com IC por bootstrap **e por fatia** — nunca um número solto.

**Entrega.** API **FastAPI** local documentada via OpenAPI.

</details>

---

## 🎓 Pesquisa acadêmica — TCC

### [UnBSense](https://github.com/luanfreitas5/UnBSense) — Mineração de dados para detecção de padrões depressivos no Twitter

> **Trabalho de Conclusão de Curso** — Bacharelado em Ciência da Computação, Universidade de Brasília (UnB)
> Inclui a [monografia completa](https://github.com/luanfreitas5/UnBSense/blob/main/Monografia_TCC.pdf) e o [artigo PIBIC](https://github.com/luanfreitas5/UnBSense/blob/main/Artigo%20PIBIC.pdf) no repositório.

Estudo de mineração de dados sobre usuários brasileiros do Twitter para detectar **sinais
comportamentais associados à depressão**, comparando dois recortes temporais: **pré-pandemia
(2018–2019)** e **pandemia (2020–2021)**.

**Contribuição.** Além dos **10 atributos comportamentais** consolidados na literatura (De Choudhury et al.),
o trabalho propõe e avalia **5 novos atributos**. Cada atributo é sumarizado em **4 vetores de
características** — média, variância, média móvel ponderada e entropia — totalizando **60 features por
dataset**.

**Metodologia.** Pipeline completo de coleta (`tweepy`, `snscrape`), pré-processamento e NLP (`NLTK`,
`spaCy`), seleção de features e seleção de modelos, avaliando um amplo conjunto de classificadores
supervisionados: **Random Forest, Gradient Boosting, SVM (RBF), MLP, AdaBoost, Bagging, KNN, LDA,
Naive Bayes, Regressão Logística e ensembles por votação** (hard/soft), com tratamento de
desbalanceamento via `class_weight` e avaliação por curvas ROC e Precision-Recall.

`Python` · `scikit-learn` · `pandas` · `NLTK` · `spaCy` · `snscrape` · `Jupyter`

---

## 🧭 Como eu trabalho

Padrões de engenharia que aplico de forma consistente em todos os projetos acima:

| Princípio | Na prática |
|---|---|
| **Métrica honesta** | PR-AUC / F1-macro com **IC 95% por bootstrap** — nunca acurácia em dado desbalanceado |
| **Sem vazamento** | Features construídas apenas com informação disponível no momento da predição; reamostragem dentro do pipeline |
| **Contratos de dados** | `Pandera` e `Pydantic` validando schema nas fronteiras do pipeline e da API |
| **Probabilidade confiável** | Calibração explícita e **Brier score**, não apenas ranqueamento |
| **Explicabilidade** | **SHAP** traduzido para linguagem de negócio, não gráfico decorativo |
| **IA Responsável** | Auditoria de fairness por subgrupo (`Fairlearn`), Model Cards e Datasheets |
| **Reprodutibilidade** | Sementes fixas, lock files, hashes de dataset, versionamento com **DVC** e rastreio no **MLflow** |
| **Qualidade de código** | `pytest` com **≥80% de cobertura**, `ruff`, `mypy`, `pre-commit` e CI no GitHub Actions |
| **Entregável real** | Todo projeto termina em **API (FastAPI)** ou **dashboard (Streamlit)** — não em notebook |

---

## 🛠️ Stack técnica

**Linguagens**

<p>
  <img src="https://skillicons.dev/icons?i=py,java,c,cpp" alt="Python, Java, C, C++" height="42" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/jupyter/jupyter-original-wordmark.svg" alt="Jupyter" height="42" />
</p>

**Dados & Processamento**

<p>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/pandas/pandas-original.svg" alt="pandas" height="42" />
  <img src="https://cdn.simpleicons.org/polars/0075FF" alt="Polars" height="42" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/numpy/numpy-original.svg" alt="NumPy" height="42" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/apachespark/apachespark-original.svg" alt="Apache Spark" height="42" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/hadoop/hadoop-original.svg" alt="Hadoop" height="42" />
  <img src="https://skillicons.dev/icons?i=mysql,mongodb,sqlite" alt="MySQL, MongoDB, SQLite" height="42" />
</p>

**Machine Learning & Deep Learning**

<p>
  <img src="https://skillicons.dev/icons?i=scikitlearn,pytorch,tensorflow" alt="scikit-learn, PyTorch, TensorFlow" height="42" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/keras/keras-original.svg" alt="Keras" height="42" />
  <img src="https://cdn.simpleicons.org/scipy/8CAAE6" alt="SciPy" height="42" />
  <img src="https://cdn.simpleicons.org/huggingface" alt="Hugging Face" height="42" />
</p>

<p>
  <img src="https://img.shields.io/badge/XGBoost-337AB7?style=flat-square&logoColor=white" alt="XGBoost" height="26" />
  <img src="https://img.shields.io/badge/LightGBM-9ACD32?style=flat-square&logoColor=white" alt="LightGBM" height="26" />
  <img src="https://img.shields.io/badge/SHAP-1F77B4?style=flat-square&logoColor=white" alt="SHAP" height="26" />
  <img src="https://img.shields.io/badge/Fairlearn-6E4B9E?style=flat-square&logoColor=white" alt="Fairlearn" height="26" />
  <img src="https://img.shields.io/badge/BERTimbau-FFB000?style=flat-square&logoColor=black" alt="BERTimbau" height="26" />
  <img src="https://img.shields.io/badge/BERTopic-4C9A2A?style=flat-square&logoColor=white" alt="BERTopic" height="26" />
  <img src="https://img.shields.io/badge/Pandera-2E7D32?style=flat-square&logoColor=white" alt="Pandera" height="26" />
</p>

**LLMs & IA Generativa**

<p>
  <img src="https://cdn.simpleicons.org/ollama" alt="Ollama" height="42" />
  <img src="https://cdn.simpleicons.org/langchain/1C3C3C" alt="LangChain" height="42" />
  <img src="https://cdn.simpleicons.org/huggingface" alt="Transformers" height="42" />
</p>

**MLOps & Deploy**

<p>
  <img src="https://cdn.simpleicons.org/mlflow/0194E2" alt="MLflow" height="42" />
  <img src="https://cdn.simpleicons.org/dvc/13ADC7" alt="DVC" height="42" />
  <img src="https://skillicons.dev/icons?i=fastapi,docker,githubactions,git" alt="FastAPI, Docker, GitHub Actions, Git" height="42" />
  <img src="https://cdn.simpleicons.org/streamlit/FF4B4B" alt="Streamlit" height="42" />
  <img src="https://skillicons.dev/icons?i=django" alt="Django" height="42" />
</p>

**Visualização & Qualidade**

<p>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/matplotlib/matplotlib-original.svg" alt="Matplotlib" height="42" />
  <img src="https://cdn.simpleicons.org/plotly/3F4F75" alt="Plotly" height="42" />
  <img src="https://cdn.simpleicons.org/pytest/0A9EDC" alt="pytest" height="42" />
  <img src="https://cdn.simpleicons.org/ruff/D7FF64" alt="Ruff" height="42" />
  <img src="https://skillicons.dev/icons?i=selenium,figma" alt="Selenium, Figma" height="42" />
</p>

---

## 📈 Atividade no GitHub

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=luanfreitas5&show_icons=true&include_all_commits=true&theme=gotham&locale=pt-br&hide_border=true" height="160" alt="Gráfico de estatísticas do GitHub" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs?username=luanfreitas5&layout=compact&theme=gotham&locale=pt-br&hide_border=true" height="160" alt="Gráfico de linguagens mais usadas" />
</div>

<div align="center">
  <img src="https://streak-stats.demolab.com?user=luanfreitas5&locale=pt-br&mode=daily&theme=gotham&hide_border=true" height="160" alt="Gráfico de sequência de commits" />
</div>

<div align="center">
  <img src="https://github-profile-trophy.vercel.app?username=luanfreitas5&theme=gotham&row=1&column=7&margin-w=8&no-frame=true&locale=pt-br" alt="Troféus de conquistas do GitHub" />
</div>

<div align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=luanfreitas5&theme=gotham&area=true&hide_border=true&locale=pt-br" alt="Gráfico de atividade de contribuições" />
</div>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/luanfreitas5/luanfreitas5/output/pacman-contribution-graph-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/luanfreitas5/luanfreitas5/output/pacman-contribution-graph.svg">
  <img alt="Gráfico animado Pac-Man de contribuições no GitHub" src="https://raw.githubusercontent.com/luanfreitas5/luanfreitas5/output/pacman-contribution-graph.svg">
</picture>

---

## 📫 Vamos conversar

Estou aberto a oportunidades e colaborações em **Ciência de Dados**, **Engenharia de Machine Learning**
e **IA Aplicada**.

<p align="left">
  <a href="https://www.linkedin.com/in/luanfreitas5/" target="_blank"><img src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/linked-in-alt.svg" alt="LinkedIn" height="30" width="40" /></a>
  <a href="https://github.com/luanfreitas5" target="_blank"><img src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/github.svg" alt="GitHub" height="30" width="40" /></a>
  <a href="https://kaggle.com/luanfreitas5" target="_blank"><img src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/kaggle.svg" alt="Kaggle" height="30" width="40" /></a>
  <a href="https://stackoverflow.com/users/luan-freitas" target="_blank"><img src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/stack-overflow.svg" alt="Stack Overflow" height="30" width="40" /></a>
  <a href="https://medium.com/luan.mgf" target="_blank"><img src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/medium.svg" alt="Medium" height="30" width="40" /></a>
  <a href="https://youtube.com/LuanVideos10" target="_blank"><img src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/youtube.svg" alt="YouTube" height="30" width="40" /></a>
  <a href="https://twitter.com/redluan21" target="_blank"><img src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/twitter.svg" alt="Twitter" height="30" width="40" /></a>
  <a href="https://instagram.com/redluan21" target="_blank"><img src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/instagram.svg" alt="Instagram" height="30" width="40" /></a>
</p>

<sub>⚡ Curiosidade: sou apaixonado por aprender algo novo de tecnologia todos os dias.</sub>
