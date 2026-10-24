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

### 🧰 Ferramentas

| Projeto | O que é | Stack principal |
|---|---|---|
| **[🧪 ds-skills](https://github.com/luanfreitas5/ds-skills)** | Coleção de 48 *skills* para Claude Code que levam agentes de IA ao padrão de um cientista de dados sênior: avaliação estatisticamente correta, dados validados, reprodutibilidade e IA responsável (LGPD, fairness) | `Claude Code` `Python` `Markdown` |

## 🚀 Projetos em destaque

Onze projetos ponta a ponta, cada um cobrindo um pilar diferente do ciclo de vida de ML —
de explicabilidade de negócio a MLOps de produção, fairness, benchmark científico, LLMs locais,
séries temporais e análise de dados públicos brasileiros.

<!-- ┌──────────────────────────────────────────────────────────────────────────┐
     │ PLACEHOLDERS DE RESULTADO — substituir cada `⬜ ...` pelo número real.    │
     │ Onde encontrar: reports/metrics/*.json de cada repositório, ou a UI do    │
     │ MLflow (`mlflow ui`). Sempre no conjunto de TESTE, nunca no de treino.    │
     │ Manter o formato "métrica valor (IC 95% a–b)" e citar sempre o baseline.  │
     └──────────────────────────────────────────────────────────────────────────┘ -->

| Projeto | Problema | Resultado principal | Stack principal |
|---|---|---|---|
| **[🔮 Previsão de Churn com Explicabilidade (Olist)](https://github.com/luanfreitas5/previsao-churn-explicavel)** | Identificar clientes com risco de não recomprar no marketplace Olist | ✅ PR-AUC `0,9919` (IC 95% `0,9897`–`0,9939`) vs. `0,9882` do baseline (CV, sem teste de significância) · ROC-AUC `0,62` · Brier `0,0720` — ⚠️ prevalência de 98,8% infla a PR-AUC | `Polars` `LightGBM` `SHAP` `Fairlearn` `MLflow` `Streamlit` |
| **[🛡️ Detecção de Fraude com Pipeline MLOps Completo](https://github.com/luanfreitas5/mlops-deteccao-fraude)** | Fraude em ~284k transações com desbalanceamento extremo (~0,17%) | ✅ PR-AUC `0,815` (IC 95% `0,732`–`0,892`) · Recall `81,1%` no limiar de custo mínimo (`0,0402`) · ROC-AUC `0,968` — baseline ainda não medido | `XGBoost` `DVC` `MLflow` `FastAPI` `Docker` `GitHub Actions` |
| **[⚖️ Predição de Risco de Diabetes com Auditoria de Justiça](https://github.com/luanfreitas5/risco-diabetes-fairness)** | Triagem de risco de diabetes a partir do BRFSS 2015 (~253k respostas) | ✅ ROC-AUC `0,8314` (IC 95% `0,8293`–`0,8335`, CV) vs. `0,8240` da regressão logística · Recall `46,9%` @ limiar 0,30 · maior disparidade de recall (escolaridade) `51 p.p.` | `LightGBM` `Fairlearn` `SHAP` `Streamlit` `Plotly` |
| **[📊 Benchmark de Análise de Sentimento em PT-BR](https://github.com/luanfreitas5/sentimento-ptbr-benchmark)** | BERTimbau realmente supera baselines clássicos? E generaliza entre domínios? | ✅ F1-macro in-domain `0,890` (BERTimbau) vs. `0,843` (TF-IDF) · fora do domínio `0,796` vs. `0,722` · gap de generalização `9,5 p.p.` vs. `12,1 p.p.` · McNemar ainda não gerado | `BERTimbau` `Transformers` `scikit-learn` `MLflow` `uv` |
| **[🤖 Análise de Emoção e Tópicos em Tweets com LLM Local](https://github.com/luanfreitas5/tweets-emocao-llm-local)** | Emoção e tópicos em ~800k tweets em português | ✅ F1-macro `0,362` (IC 95% `0,361`–`0,363`; baseline trivial `0,266`) · meta de `0,70` não atingida · `31` tópicos, porém modelagem degenerada (37,9% outliers) · tweets/s não medido | `BERTopic` `Ollama` `Llama 3.1` `FastAPI` `Pydantic` |
| **[📈 Simulador do Tesouro Direto](https://github.com/luanfreitas5/simulador-tesouro-direto)** | Quanto sobra ao investidor após imposto, custódia e inflação? Curva de juros histórica e rentabilidade bruta, líquida e real | ✅ Pipeline em ~5 s sobre `177.434` preços (2004–2026) com contratos Pandera aprovados · curva Prefixada **invertida** em 15/10/2026 (`13,37%` em 0,2 ano vs. `12,64%` em 2,2 anos) e IPCA+ plana (`6,7%`–`6,8%` real) · simulador bruto/líquido/real vs. Selic | `Polars` `Pandera` `uv` `GitHub Actions` `MkDocs` |
| **[🏛️ Mapa Temático do Congresso](https://github.com/luanfreitas5/mapa-tematico-congresso-nlp)** | Quais temas dominam a Câmara dos Deputados (57ª legislatura) e quem são os atores centrais nas redes de coautoria e de votos? | ✅ Coerência c_v `0,739` (IC 95% `0,702`–`0,774`) em `17.482` ementas (`122` tópicos, 25,3% de ruído) e `0,666` em `44.269` discursos (`125` tópicos, 54,1% de ruído) · rede de coautoria com `617` deputados e `9.230` arestas · rede de votos com `22` partidos em `2` comunidades | `BERTopic` `sentence-transformers` `NetworkX` `Pandera` |
| **[📉 Previsão do IPCA com Backtest Walk-Forward](https://github.com/luanfreitas5/previsao-ipca-backtest)** | Algum modelo, usando só informação disponível na data, supera o Boletim Focus na previsão do IPCA mensal? | ✅ Nenhum modelo superou o Focus: RMSE `0,257` (IC 95% `0,220`–`0,293`) vs. `0,334` do melhor modelo (AutoARIMA) em 1 mês (Diebold-Mariano p < 0,001); empate estatístico em 6 e 12 meses | `statsforecast` `LightGBM` `MLflow` `Pandera` |
| **[🎓 Radar da Educação Municipal](https://github.com/luanfreitas5/radar-educacao-municipal)** | Que tipologias de município emergem de infraestrutura escolar e contexto socioeconômico? O IDEB se agrupa no território? | ✅ `4` tipologias estáveis (ARI `0,98`, IC 95% `0,95`–`0,99`; ⚠️ silhouette baixa, `0,189`) · IDEB difere entre grupos (Kruskal-Wallis, ε² `0,24` anos iniciais / `0,19` finais) · autocorrelação espacial forte (I de Moran `0,625` / `0,591`) | `scikit-learn` `UMAP` `geobr` `Polars` |
| **[🎯 Desempenho no ENEM e Equidade](https://github.com/luanfreitas5/desempenho-enem-equidade)** | Quanto o perfil socioeconômico explica a nota do ENEM, e o erro do modelo é equânime entre grupos? | ✅ R² `0,330` (IC 95% `0,325`–`0,335`) com XGBoost vs. `0,319` do OLS (RMSE `70,98`) · perfil socioeconômico explica só ~33% da variância · renda e computador dominam o SHAP · gap de renda (até 1 SM vs. mais de 6 SM) `−128,9` pontos · modelo superestima indígenas (`+32,5`) e escola pública (`+15,0`) | `Polars` `XGBoost` `SHAP` `Fairlearn` |
| **[💹 Painel Macro BCB](https://github.com/luanfreitas5/painel-macro-bcb)** | O quanto a mediana do Focus erra o IPCA mensal, e há viés sistemático por horizonte? | ✅ MAE do Focus cresce de `0,082` p.p. (mês corrente) para `0,265` p.p. (12 meses) e satura · viés levemente negativo (`−0,088` p.p. em 12 meses, IC exclui zero) · ⚠️ ICs ignoram autocorrelação dos erros | `Streamlit` `Polars` `python-bcb` `uv` |

<sub>✅ = valores extraídos dos READMEs de cada repositório (em 24/10/2026). Itens marcados como ausentes ainda estão pendentes nos respectivos projetos.</sub>

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

**Diferencial.** SHAP traduzido para linguagem de negócio + auditoria de fairness por UF.

**Entrega.** Dashboard **Streamlit** que traduz os valores SHAP em explicações de negócio por cliente —
transformando score em decisão de retenção acionável.

> **✅ Resultados** (teste, split 80/20 estratificado, semente 42; IC por bootstrap de 1.000 reamostragens).
>
> - PR-AUC: `0,9919` — IC 95% `[0,9897 ; 0,9939]` · ROC-AUC `0,6214`
> - Baseline (`DummyClassifier`, CV no treino): PR-AUC `0,9882` → ganho de `0,2 p.p.`, da ordem do próprio IC; **sem teste de significância**, então não se afirma que o modelo é "melhor"
> - Brier score: `0,0720` — ⚠️ com `class_weight="balanced"` e prevalência de ~99%, as probabilidades não são calibradas
> - Menor recall por UF: TO `0,865`, AM `0,882` e GO `0,916` vs. SP `0,928` (⚠️ sem `n` por UF, a amplitude de `0,135` não é interpretável)
> - Top-3 drivers de churn por SHAP: UF do cliente (`0,58`), dias desde a última compra (`0,34`), frete médio (`0,28`)

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

> **✅ Resultados** (teste, split estratificado 60/20/20, semente 42; limiar escolhido na validação).
>
> - PR-AUC: `0,815` — IC 95% `[0,732 ; 0,892]` · ROC-AUC `0,968` · Brier `0,0004`
> - Baseline (Regressão Logística): **não medido** com o mesmo protocolo e sem teste de significância — não se afirma ganho
> - Limiar ótimo por custo: `0,0402` → recall `81,1%` com precisão `72,6%` (F1 `0,766`)
> - ⚠️ ICs largos: há poucas dezenas de fraudes por partição
> - Pior segmento, fraudes capturadas vs. 0.5 padrão, latência da API e cobertura: não avaliados/medidos ainda

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

> **✅ Resultados** (split estratificado 60/20/20, semente 42; CV de 5 folds no treino).
>
> - ROC-AUC: CV `0,8314` — IC 95% `[0,8293 ; 0,8335]` · holdout `0,8272` (pontual, ⚠️ bootstrap pendente)
> - PR-AUC (prevalência ~14%): `0,4235` no holdout
> - No limiar 0,30: recall `46,9%` · precisão `43,2%` · F1 `0,450`
> - Baseline (Regressão Logística): ROC-AUC CV `0,8240` → ganho de `0,74 p.p.`; teste de significância ainda não feito
> - Brier após calibração isotônica (holdout): `0,0973` (antes da calibração: não reportado)
> - Fairness — maior gap de recall: escolaridade `51 p.p.`, renda `37 p.p.`, idade `35 p.p.` (jovens 18–39 com recall `0,159`), sexo `0,8 p.p.`

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

> **✅ Resultados** (`20.000` amostras por domínio, split 80/20, semente 42; IC 95% por bootstrap de 1.000 reamostragens).
>
> - F1-macro médio **in-domain**: BERTimbau `0,890` vs. TF-IDF+LR `0,843`
> - F1-macro médio **out-of-domain**: BERTimbau `0,796` vs. TF-IDF+LR `0,722`
> - **Gap de generalização**: BERTimbau `9,5 p.p.` · baseline `12,1 p.p.`
> - Domínio mais difícil: `utlc_movies` (in-domain `0,817` / `0,747`); pior célula: BERTimbau `utlc_movies → olist` (`0,600`)
> - Melhor in-domain: `b2w` — BERTimbau `0,955` (IC 95% `0,947`–`0,962`) vs. `0,914`; ICs não se sobrepõem nos 5 domínios, mas **não é teste formal**
> - McNemar (BERTimbau vs. baseline): ainda não gerado neste snapshot
> - ⚠️ Uma única semente e um split por domínio: variância entre treinos não quantificada · custo de fine-tuning não medido

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

> **✅ Resultados** (avaliação sem treino sobre `713.518` tweets limpos, referência = emoticon, ruidosa; execução de 24/10/2026).
>
> - F1-macro (3 classes): `0,362` — IC 95% `[0,361 ; 0,363]` · baseline trivial ("sempre Negativo") `0,266` · 2 classes `0,543` · meta `0,70` **não atingida**
> - ⚠️ A acurácia do modelo (`55,3%`) é menor que a de responder sempre "Negativo" (`66,2%`); a classe Neutro tem suporte `0` na referência
> - Pior fatia: tweets curtos (1–5 palavras) com F1 `0,334`, contra `0,374` em 16+ palavras
> - Tópicos (BERTopic): `31`, porém modelagem degenerada — `37,9%` outliers e `60,7%` em um único tópico (`98,5%` sem tópico informativo)
> - Geração local (`llama3.1:8b`): `1 min 59 s` para o resumo · throughput em tweets/s não medido
> - Baseline TF-IDF + regressão logística: pendente

---

### 📈 [simulador-tesouro-direto](https://github.com/luanfreitas5/simulador-tesouro-direto) — Quanto sobra depois do imposto e da inflação

**Problema.** Taxas de títulos públicos são divulgadas como "X% ao ano" ou "IPCA + X%", mas o que importa
ao investidor é o rendimento **depois de imposto, custódia e inflação**. Comparar Prefixado, IPCA+ e a
Selic exige juntar a taxa contratada, a inflação do período e as regras tributárias.

**Abordagem.** Arquitetura medalhão (bronze → silver → gold) sobre Tesouro Transparente e BCB SGS
(Selic e IPCA). A ingestão é **idempotente**, com cache local (TTL de 24 h), snapshots imutáveis e
manifesto SHA-256; se a rede falhar, reutiliza o último snapshot com aviso.

**Rigor.** Contratos de dados com `Pandera` em cada camada e parâmetros financeiros (alíquotas, custódia)
em `configs/finance.yaml`, não no código. Premissas para o trecho sem dado observado são declaradas como
do usuário, **não** como previsões.

**Entrega.** App com curva de juros navegável por data e simulador com cascata *investido → bruto → IR →
custódia → líquido* e comparação com a Selic no mesmo valor e prazo.

> **✅ Resultados** (execução de 17/10/2026).
>
> - Pipeline completo em ~`5 s` sobre `177.434` preços (31/12/2004 a 15/10/2026); gold com `47.157` pontos de curva
> - Curva Prefixada **invertida** em 15/10/2026: `13,37%` a.a. em 0,2 ano vs. `12,64%` em 2,2 anos
> - Curva real do IPCA+ praticamente plana: `6,7%`–`6,8%` a.a.
> - ⚠️ Projeto educacional, sem recomendação de investimento

---

### 🏛️ [mapa-tematico-congresso-nlp](https://github.com/luanfreitas5/mapa-tematico-congresso-nlp) — Temas e redes na Câmara dos Deputados

**Problema.** A Câmara produz milhares de proposições, votações e discursos por ano. Sem visão estruturada,
é difícil saber quais temas dominam a agenda, como evoluem e como os atores se relacionam.

**Abordagem.** Dados abertos da API oficial (57ª legislatura) em camadas bronze → silver → gold.
Embeddings + **BERTopic** sobre ementas e discursos, e redes com **NetworkX**: coautoria entre deputados e
alinhamento de votos entre partidos.

**Rigor.** Coerência de tópicos (`c_v` e `c_npmi`) com **IC 95% por bootstrap** sobre os tópicos,
sementes fixas, `uv.lock` e hash SHA-256 de cada snapshot. Foto e e-mail dos deputados são descartados na
silver (minimização, LGPD) e há datasheet da fonte.

**Entrega.** Evolução temporal dos tópicos, métricas de centralidade (força e intermediação) e
comunidades das duas redes.

> **✅ Resultados** (snapshot da API de 22/10/2026, semente 42).
>
> - Ementas (`17.482` documentos): `122` tópicos, `c_v` `0,739` (IC 95% `0,702`–`0,774`), `25,3%` de ruído
> - Discursos (`44.269` documentos): `125` tópicos, `c_v` `0,666` (IC 95% `0,639`–`0,693`), `54,1%` de ruído
> - Coautoria: `617` deputados, `9.230` arestas, `172` comunidades (`7` grandes)
> - Votos: `22` partidos, `199` arestas (~86% de densidade), `2` comunidades — a densidade limita o poder discriminativo da centralidade
> - ⚠️ Revisão manual de coerência ainda não rotulada; só a coerência automática está disponível

---

### 📉 [previsao-ipca-backtest](https://github.com/luanfreitas5/previsao-ipca-backtest) — Previsão de inflação sem vazamento temporal

**Problema.** Avaliar previsão de inflação costuma ser enganoso: usar séries na versão final (ignorando a
data de divulgação), treinar com alvos ainda desconhecidos ou comparar modelos em amostras diferentes gera
erros artificialmente baixos.

**Abordagem.** Features **point-in-time**: na origem `o`, só entram observações com `available_at <= o`,
com atrasos de divulgação por série. Modelos: ingênuos, `AutoARIMA`, `AutoETS` (statsforecast) e
`LightGBM` direto por horizonte, em backtest **walk-forward** de janela expansiva (1, 2, 3, 6 e 12 meses).

**Rigor.** Referência é a mediana do **Boletim Focus**. Amostra comum a todos os modelos, RMSE com IC 95%
por bootstrap em blocos, teste de **Diebold-Mariano** (correção HLN) e intervalos **conformais** de 90%.
Testes automatizados alteram valores futuros e exigem que as features não mudem.

**Entrega.** Execuções no **MLflow** (SHA do Git e hashes dos dados) e relatório final com piores erros e
fatias por subperíodo.

> **✅ Resultados.**
>
> - h=1: Focus RMSE `0,257` (IC 95% `0,220`–`0,293`) vs. `0,334` do AutoARIMA e `0,412` do ingênuo (Diebold-Mariano p < `0,001`)
> - h=6 e h=12: AutoARIMA empata estatisticamente com o Focus (p = `0,65` e `0,44`, perda quadrática)
> - LightGBM (`0,363` em h=1) não supera o AutoARIMA, apesar das features extras
> - ⚠️ Cobertura conformal nominal de 90% fica em `0,77`–`0,89`: intervalos subcobrem em períodos de choque

---

### 🎓 [radar-educacao-municipal](https://github.com/luanfreitas5/radar-educacao-municipal) — Tipologias de municípios e análise espacial

**Problema.** Os 5.570 municípios diferem muito em infraestrutura escolar, porte e renda, mas as políticas
costumam tratá-los como um bloco homogêneo. Falta uma visão integrada de quais perfis existem e se ocupam
o território de forma agrupada.

**Abordagem.** Integra **Censo Escolar**, **IDEB** e **IBGE** pela chave de 7 dígitos do município, com
testes de integridade (duplicatas, chaves órfãs, cobertura mínima). Clusterização com `KMeans` (k por
silhouette) e `UMAP` **apenas** para visualização; autocorrelação com **I de Moran** e **LISA**.

**Rigor.** O IDEB **não entra** na clusterização, então serve como validação externa: IC 95% bootstrap por
cluster e teste de Kruskal-Wallis com tamanho de efeito (ε²). Estabilidade dos grupos por subamostragem (ARI).

**Entrega.** Relatório reprodutível (`make reproduce`) com figuras 300 dpi + SVG e datasheet da base municipal.

> **✅ Resultados.**
>
> - `4` tipologias; estabilidade ARI `0,98` (IC 95% `0,95`–`0,99`)
> - ⚠️ Silhouette `0,189`: grupos se sobrepõem e devem ser lidos como perfis, não como categorias separadas
> - IDEB difere entre grupos: ε² `0,24` (anos iniciais) e `0,19` (anos finais)
> - Autocorrelação espacial: I de Moran `0,625` (anos iniciais) e `0,591` (anos finais)
> - Cluster crítico (`111` municípios, infraestrutura precária, região Norte): IDEB mediano `4,6` vs. `6,1`–`6,2` nos grupos 1 e 2

---

### 🎯 [desempenho-enem-equidade](https://github.com/luanfreitas5/desempenho-enem-equidade) — Explicabilidade e equidade no ENEM

**Problema.** A nota do ENEM é fortemente associada às condições socioeconômicas. Quantificar essa
associação — e checar se o modelo erra mais para alguns grupos — é um passo básico para qualquer uso
responsável de dados educacionais.

**Abordagem.** Microdados do ENEM (2022 e 2023) lidos de forma **lazy** com Polars e gravados em Parquet
particionado por ano. Features apenas do questionário socioeconômico; raça/cor, tipo de escola e região
**não** entram no modelo e servem para agrupar a análise de equidade. Comparação **OLS vs. XGBoost** com **SHAP**.

**Rigor.** Notas, gabaritos e presença são bloqueados como feature por código (`validate_no_leakage`) e
por teste. Todos os intervalos são IC 95%; a diferença entre modelos usa bootstrap e teste *t* corrigido na CV.

**Entrega.** Tabelas de desempenho, importância SHAP, desigualdade de nota e viés do modelo por grupo,
além de datasheet e dicionário de dados.

> **✅ Resultados** (teste, n = `100 mil`; `3.945.675` candidatos após o funil).
>
> - XGBoost: R² `0,330` (IC 95% `0,325`–`0,335`), RMSE `70,98` · OLS: R² `0,319`, RMSE `71,59`
> - Ganho do boosting pequeno: RMSE `0,61` ponto menor (*p* = `6,6·10⁻⁶`, 5 folds)
> - Top SHAP: renda familiar (`20,7` pontos), computador (`14,2`), escolaridade da mãe (`6,8`)
> - Até 1 SM vs. mais de 6 SM: `−128,9` pontos (IC 95% `−130,7`–`−127,2`)
> - Viés (previsto − observado): indígenas `+32,5`, pretos `+15,7`, escola pública `+15,0` — não é evidência causal
> - ⚠️ Indígenas têm `n = 517`, com IC largo

---

### 💹 [painel-macro-bcb](https://github.com/luanfreitas5/painel-macro-bcb) — Indicadores do BCB e erro do Focus

**Problema.** Decisões de investimento e política econômica dependem de indicadores espalhados em APIs
distintas e com frequências diferentes. A inflação esperada pelo mercado (Focus) é usada como referência,
mas raramente se mede o quanto ela acerta.

**Abordagem.** Séries do BCB (Meta Selic, IPCA, dólar e expectativas do Focus) via `python-bcb`, em camadas
bronze → silver → gold, com consulta de séries diárias por janelas de data (limite de 10 anos da API do SGS).
Transformações em `Polars`; IPCA em 12 meses por composição.

**Rigor.** Erro do Focus = mediana projetada − IPCA realizado, por horizonte de 0 a 12 meses, com viés, MAE
e RMSE e IC 95%. Contratos de dados e ingestão idempotente com manifesto SHA-256.

**Entrega.** Dashboard **Streamlit** (`make app`) com os indicadores e a análise do erro do Focus.

> **✅ Resultados** (coleta de 17/10/2026; painel de jan/2010 a out/2026, `202` meses).
>
> - MAE do Focus: `0,082` p.p. no mês corrente → `0,244` (3 meses) → `0,265` (12 meses), saturando
> - Viés levemente negativo: `−0,088` p.p. em 12 meses (IC 95% exclui zero), cerca de um terço do MAE — o erro é dominado por dispersão
> - ⚠️ ICs ignoram a autocorrelação dos erros e são otimistas

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

<!-- PREENCHER: números da Monografia_TCC.pdf / Artigo PIBIC.pdf. -->
> **⬜ Resultados.**
>
> - Usuários coletados: `__` (`__` no grupo depressivo / `__` no controle)
> - Melhor classificador: `___` — acurácia `__%` · F1 `0,__` · AUC `0,__`
> - Desempenho pré-pandemia vs. pandemia: `0,__` vs. `0,__`
> - Contribuição dos **5 novos atributos**: `+__ p.p.` sobre o conjunto de De Choudhury
> - Atributos mais discriminativos na seleção de features: `___`, `___`, `___`

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
