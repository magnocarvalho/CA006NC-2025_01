# Análise de Dados Públicos: Assistência Financeira e Criminalidade em Minas Gerais
# CA006NC - Inteligência Artificial - (2025_01)
--

### **Título Provisório**

> *Correlação entre Assistência Financeira e Criminalidade em Municípios de Minas Gerais: Uma Abordagem com IA sobre Dados Públicos de Bolsa Família, Pix e Violência*

---

### **Resumo**


* Contexto: disparidades econômicas, insegurança pública.
* Objetivo: investigar se existe relação entre assistência financeira (Bolsa Família + Pix) e crimes violentos.
* Metodologia: uso de clustering, análise de séries temporais e correlação entre variáveis socioeconômicas.
* Resultados: principais achados sobre aumento de crimes em períodos de menor repasse.
* Conclusão: possíveis implicações para políticas públicas.

---

### **1. Introdução**

* **Contexto**: desigualdade social, importância de transferências de renda no Brasil.
* **Problema de Pesquisa**: será que a oscilação ou escassez de recursos financeiros (via Bolsa Família ou fluxo Pix) está correlacionada ao aumento de crimes violentos?
* **Objetivo**: explorar essa correlação com IA aplicada a dados de municípios mineiros.
* **Resumo da Metodologia**: coleta de três bases, uso de normalização e clustering, análise de correlação.
* **Estrutura do Artigo**: seção 2 traz os trabalhos relacionados, seção 3 a metodologia, etc.

---

### **2. Trabalhos Relacionados**

* Estudo sobre o impacto do Bolsa Família na redução da criminalidade (ex: Neri e Soares, IPEA).
* Uso de séries temporais e IA para prever criminalidade (ex: LSTM em segurança pública).
* Artigos sobre análise de comportamento econômico via Pix e open finance.

---

### **3. Metodologia**

**a. Bases de Dados**

* *Bolsa Família*: valores pagos por município/mês (Portal da Transparência)
* *Indicadores de Violência*: crimes por município/mês (SINESP ou base SES-MG)
* *Pix*: volume e número de transações por município/mês (BCB)

**b. Pré-processamento**

* Normalização por 100 mil habitantes
* Ajustes temporais (defasagens entre pagamentos e crimes)
* Unificação por código IBGE dos municípios

**c. Técnicas de IA**

* Clustering com K-Means para agrupar municípios semelhantes
* Regressão linear, correlação (Pearson/Spearman)
* Modelagem temporal (média móvel, Prophet ou LSTM, se possível)

**d. Avaliação**

* Visualizações: mapas de calor, gráficos de linha, correlogramas
* Métricas de desempenho para predições (R², RMSE, etc.)

---

### **4. Resultados Experimentais**

* Gráficos de série temporal mostrando picos de crimes após períodos com queda em benefícios.
* Correlações significativas entre menor fluxo de Pix e maior número de ocorrências.
* Clusters de municípios vulneráveis (baixo Pix + alto crime)
* Discussão sobre sazonalidade (ex: aumento de crimes no fim do mês)

---

### **5. Conclusão**

* Confirmação (ou não) da hipótese inicial.
* Destaque: municípios com menor circulação de recursos tendem a apresentar mais violência?
* Contribuições: uso de IA em política pública.
* Limitações: qualidade dos dados, granularidade temporal.
* Trabalhos futuros: inclusão de mais variáveis (escolaridade, dados climáticos, etc.), outros estados.
