
<article class="markdown-body entry-content container-lg" itemprop="text"><div class="markdown-heading" dir="auto"><h1 tabindex="-1" class="heading-element" dir="auto">Análise de Churn Telecom X</h1><a id="user-content-análise-de-churn-telecom-x" class="anchor" aria-label="Permalink: Análise de Churn Telecom X" href="#análise-de-churn-telecom-x"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto">Eu sou <strong>Higor Barreto</strong> e este projeto consiste em uma análise da evasão de clientes (Churn) na empresa Telecom X.</p>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto">Objetivo do Projeto</h2><a id="user-content-objetivo-do-projeto" class="anchor" aria-label="Permalink: Objetivo do Projeto" href="#objetivo-do-projeto"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto">O principal objetivo deste projeto é:</p>
<ul dir="auto">
<li><strong>Compreender o problema de Churn:</strong> Quantificar a taxa de evasão e sua distribuição dentro da base de clientes da Telecom X.</li>
<li><strong>Identificar os principais drivers de Churn:</strong> Descobrir quais características dos clientes, tipos de serviço e padrões de comportamento estão mais associados ao cancelamento do serviço.</li>
<li><strong>Fornecer insights estratégicos:</strong> Gerar recomendações baseadas em dados para ajudar a Telecom X a reduzir sua taxa de Churn e, consequentemente, aumentar a retenção de clientes e a receita.</li>
</ul>
<hr>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto">Metodologia</h2><a id="user-content-metodologia" class="anchor" aria-label="Permalink: Metodologia" href="#metodologia"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto">A análise seguiu uma metodologia estruturada para garantir a clareza dos resultados:</p>
<ul dir="auto">
<li><strong>Importação dos Dados:</strong> Coleta e carregamento dos dados de uma API externa.</li>
<li><strong>Limpeza e Tratamento de Dados (Feature Engineering):</strong> Preparação dos dados para análise, incluindo normalização de estruturas aninhadas, tratamento de valores ausentes, padronização de variáveis binárias, aplicação de One-Hot Encoding para variáveis categóricas e criação de novas features relevantes (<code>Contas_Diarias</code>).</li>
<li><strong>Exploração e Análise:</strong> Investigação detalhada das variáveis, tanto numéricas quanto categóricas, em relação à variável alvo <code>Churn</code>.</li>
<li><strong>Visualização:</strong> Criação de gráficos (barras, distribuição) para ilustrar padrões, proporções e relacionamentos entre as variáveis.</li>
<li><strong>Conclusões e Recomendações:</strong> Resumo dos principais insights e proposição de estratégias acionáveis para mitigar o problema de churn.</li>
</ul>
<hr>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto">Ferramentas Utilizadas</h2><a id="user-content-ferramentas-utilizadas" class="anchor" aria-label="Permalink: Ferramentas Utilizadas" href="#ferramentas-utilizadas"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto">Este projeto foi desenvolvido utilizando as seguintes ferramentas e bibliotecas:</p>
<ul dir="auto">
<li><strong>Python</strong></li>
<li><strong>Jupyter Notebook / Google Colab</strong></li>
<li><strong>Pandas:</strong></li>
<li><strong>Matplotlib</strong></li>
<li><strong>Seaborn</strong></li>
<li><strong>Numpy</strong></li>
</ul>
<hr>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto">Etapas da Análise Detalhada</h2><a id="user-content-etapas-da-análise-detalhada" class="anchor" aria-label="Permalink: Etapas da Análise Detalhada" href="#etapas-da-análise-detalhada"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto">O projeto foi estruturado nas seguintes fases:</p>
<ol dir="auto">
<li>
<p dir="auto"><strong>Coleta e Importação de Dados:</strong> Os dados foram obtidos a partir de uma API, contendo informações detalhadas sobre clientes, serviços telefônicos, serviços de internet e detalhes da conta.</p>
</li>
<li>
<p dir="auto"><strong>Limpeza e Tratamento de Dados (Feature Engineering):</strong></p>
<ul dir="auto">
<li><strong>Normalização de Dados Aninhados:</strong> Estruturas JSON aninhadas foram "achatadas" para criar um <code>DataFrame</code> plano e fácil de trabalhar.</li>
<li><strong>Tratamento de Valores Ausentes:</strong> Identificação e tratamento de valores ausentes (NaNs), especialmente em colunas numéricas, como <code>account_Charges.Total</code>.</li>
<li><strong>Padronização da Variável Alvo (<code>Churn</code>):</strong> A variável <code>Churn</code> foi convertida de categorias textuais ('Yes'/'No') para valores numéricos binários (1/0).</li>
<li><strong>Mapeamento de Variáveis Binárias:</strong> Colunas categóricas binárias foram mapeadas para 0s e 1s para facilitar a análise e modelagem.</li>
<li><strong>One-Hot Encoding:</strong> Variáveis categóricas com múltiplas opções (e.g., tipo de contrato, método de pagamento, serviço de internet) foram transformadas usando One-Hot Encoding, criando colunas indicadoras.</li>
<li><strong>Criação de Novas Features:</strong> Uma nova coluna, <code>Contas_Diarias</code>, foi criada para representar o custo médio diário do serviço, oferecendo uma granularidade adicional.</li>
</ul>
</li>
<li>
<p dir="auto"><strong>Análise Exploratória de Dados (EDA):</strong></p>
<ul dir="auto">
<li><strong>Análise Descritiva:</strong> Geração de estatísticas descritivas para entender a distribuição e o comportamento das variáveis numéricas e categóricas.</li>
<li><strong>Visualização da Distribuição de Churn:</strong> Gráficos para entender a proporção de clientes que cancelaram vs. permaneceram.</li>
<li><strong>Análise de Churn por Variáveis Categóricas:</strong> Visualização e quantificação da taxa de churn em relação a diversos atributos do cliente e serviço (gênero, tipo de contrato, serviços adicionais, método de pagamento, etc.). Isso incluiu a criação de múltiplos gráficos de barras com porcentagens claras, além de um resumo textual detalhado desses insights.</li>
</ul>
</li>
</ol>
<hr>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto">Conclusões e Insights</h2><a id="user-content-conclusões-e-insights" class="anchor" aria-label="Permalink: Conclusões e Insights" href="#conclusões-e-insights"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto">A análise revelou padrões associados ao churn:</p>
<ul dir="auto">
<li><strong>Taxa de Churn Elevada:</strong> A Telecom X apresenta uma taxa de churn geral de <strong>26.54%</strong>, indicando uma área crítica para intervenção.</li>
<li><strong>Contratos Mês a Mês:</strong> Clientes com <strong>contrato <code>Month-to-month</code></strong> são o principal driver de churn, com uma taxa de <strong>42.71%</strong>, comparado a apenas 6.76% para outros tipos de contrato. A falta de compromisso de longo prazo é um fator de alto risco.</li>
<li><strong>Método de Pagamento (Cheque Eletrônico):</strong> Clientes que utilizam <strong><code>Electronic check</code></strong> como método de pagamento apresentam uma taxa de churn alarmante de <strong>45.29%</strong>, significativamente maior que outros métodos (17.06%).</li>
<li><strong>Serviço de Internet (Fibra Óptica):</strong> Clientes com <strong><code>Fiber optic</code></strong> têm uma taxa de churn de <strong>41.89%</strong>, quase o triplo dos clientes sem fibra (14.49%). Isso sugere problemas de qualidade no serviço de fibra ou uma base de clientes mais exigente.</li>
<li><strong>Senior Citizens:</strong> Clientes <strong><code>SeniorCitizen</code></strong> (idosos) mostram uma taxa de churn de <strong>41.68%</strong>, quase o dobro dos não-idosos (23.61%).</li>
<li><strong>Faturamento Sem Papel (<code>PaperlessBilling</code>):</strong> Clientes que optam por faturas sem papel (<code>Yes</code>) têm o dobro da taxa de churn (33.57%) comparado aos que recebem fatura impressa (16.33%).</li>
<li><strong>Fatores Protetores (Menor Churn):</strong>
<ul dir="auto">
<li><strong>Contratos de Dois Anos (<code>Two year</code>):</strong> Churn de apenas <strong>2.83%</strong>.</li>
<li><strong>Serviços Adicionais:</strong> Clientes com <strong><code>OnlineSecurity</code></strong> (14.61%) e <strong><code>TechSupport</code></strong> (15.17%) têm taxas de churn consideravelmente mais baixas. Isso demonstra o valor percebido desses serviços.</li>
<li><strong>Clientes com Família:</strong> Clientes com <strong><code>Partner</code></strong> (19.66%) e <strong><code>Dependents</code></strong> (15.45%) são mais propensos a permanecer.</li>
</ul>
</li>
</ul>
<hr>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto">Recomendações</h2><a id="user-content-recomendações" class="anchor" aria-label="Permalink: Recomendações" href="#recomendações"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto">Com base nas conclusões, as seguintes ações são recomendadas para a Telecom X:</p>
<ol dir="auto">
<li><strong>Fortalecer a Fidelização:</strong> Implementar programas de incentivo para migrar clientes de contratos mensais para anuais/bianuais, oferecendo descontos atrativos ou benefícios exclusivos.</li>
<li><strong>Atenção ao Cliente de Fibra Óptica e Cheque Eletrônico:</strong>
<ul dir="auto">
<li>Realizar pesquisas de satisfação e auditorias de qualidade para clientes de fibra óptica.</li>
<li>Oferecer planos de fidelidade ou suporte personalizado para clientes que pagam via cheque eletrônico.</li>
</ul>
</li>
<li><strong>Suporte e Ofertas para Idosos:</strong> Desenvolver canais de atendimento mais acessíveis, materiais explicativos simplificados e pacotes de serviços que atendam às necessidades específicas do usuário idoso.</li>
<li><strong>Promover Serviços de Valor Agregado:</strong> Campanhas de marketing devem destacar os benefícios da segurança online e do suporte técnico, incentivando a adesão a esses serviços como forma de aumentar a satisfação e a retenção.</li>
<li><strong>Reavaliar a Experiência da Fatura Digital:</strong> Investigar o motivo do maior churn em clientes com fatura sem papel, buscando otimizar a comunicação digital e a experiência do usuário para esse segmento.</li>
</ol>
<hr>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto">Desenvolvido por 💼</h2><a id="user-content-desenvolvido-por-" class="anchor" aria-label="Permalink: Desenvolvido por 💼" href="#desenvolvido-por-"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto">Higor Francisco Fulaneti Barreto</p>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto">Agradecimentos</h3><a id="user-content-agradecimentos" class="anchor" aria-label="Permalink: Agradecimentos" href="#agradecimentos"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto">Agradeço à <strong>Oracle Next Education (ONE)</strong> e à <strong>Alura</strong> pelo desafio e oportunidade de aprendizado.</p>
</article>
