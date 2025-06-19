# 📊 Análise de Churn - Telecom X

**Autor:** Higor Francisco Fulaneti Barreto  
**Objetivo:** Este projeto consiste em uma análise da evasão de clientes (*Churn*) na empresa fictícia **Telecom X**.

---

## 🎯 Objetivos do Projeto

- 📉 **Compreender o problema de Churn:** Quantificar a taxa de evasão e sua distribuição dentro da base de clientes da Telecom X.  
- 🔍 **Identificar os principais drivers de Churn:** Descobrir quais características dos clientes, tipos de serviço e padrões de comportamento estão mais associados ao cancelamento do serviço.  
- 💡 **Fornecer insights estratégicos:** Gerar recomendações baseadas em dados para ajudar a empresa a reduzir sua taxa de churn e aumentar a retenção de clientes e a receita.

---

## 🧠 Metodologia

A análise seguiu uma metodologia estruturada para garantir a clareza dos resultados:

1. **Importação dos Dados:** Coleta de dados a partir de uma API externa.
2. **Limpeza e Tratamento de Dados (Feature Engineering):**
   - Normalização de estruturas aninhadas (JSON).
   - Tratamento de valores ausentes.
   - Padronização de variáveis binárias.
   - One-Hot Encoding para variáveis categóricas.
   - Criação de novas variáveis como `Contas_Diarias`.
3. **Exploração e Análise:** Investigação detalhada das variáveis em relação ao `Churn`.
4. **Visualização de Dados:** Gráficos para identificar padrões e relações.
5. **Conclusões e Recomendações:** Geração de insights e ações estratégicas.

---

## 🛠️ Ferramentas Utilizadas

- Python  
- Jupyter Notebook / Google Colab  
- Pandas  
- Numpy  
- Matplotlib  
- Seaborn  

---

## 🔬 Etapas da Análise Detalhada

### 📥 Coleta e Importação de Dados

Os dados foram obtidos via API, contendo informações sobre clientes, serviços contratados e contas.

### 🧹 Limpeza e Feature Engineering

- **Normalização:** Estruturas JSON aninhadas foram "achatadas" para criar um DataFrame plano.
- **Valores Ausentes:** Tratamento de NaNs, especialmente em colunas como `account_Charges.Total`.
- **Churn:** Conversão de 'Yes'/'No' para 1/0.
- **Variáveis Binárias:** Mapeadas para 0s e 1s.
- **One-Hot Encoding:** Para colunas com múltiplas categorias.
- **Nova Feature:** `Contas_Diarias` criada para representar o custo médio diário.

### 📊 Análise Exploratória de Dados (EDA)

- Estatísticas descritivas.
- Gráficos de distribuição e proporção de Churn.
- Comparações por categoria (ex: contrato, método de pagamento, idade, etc.).

---

## 📈 Principais Insights

### 🚨 Fatores de Risco para o Churn

| Fator | Taxa de Churn |
|-------|----------------|
| Contrato Mês a Mês | 42.71% |
| Cheque Eletrônico | 45.29% |
| Fibra Óptica | 41.89% |
| Clientes Idosos | 41.68% |
| Fatura Digital (Paperless) | 33.57% |

### ✅ Fatores Protetores (Menor Churn)

| Fator | Taxa de Churn |
|-------|----------------|
| Contrato de 2 anos | 2.83% |
| OnlineSecurity Ativo | 14.61% |
| TechSupport Ativo | 15.17% |
| Clientes com Parceiro | 19.66% |
| Clientes com Dependentes | 15.45% |

---

## 💡 Recomendações Estratégicas

- **Fidelização de Clientes:** Incentivar a migração para contratos mais longos com benefícios ou descontos.
- **Clientes de Fibra e Cheque Eletrônico:** Oferecer suporte personalizado e investigar insatisfação.
- **Atenção a Idosos:** Criar canais acessíveis, suporte humanizado e pacotes mais amigáveis.
- **Promoção de Serviços Adicionais:** Destacar OnlineSecurity e TechSupport como diferenciais de valor.
- **Revisão da Fatura Digital:** Melhorar experiência digital para reduzir evasão.

---

## 🙏 Agradecimentos

Agradeço à **Oracle Next Education (ONE)** e à **Alura** pelo desafio e pela oportunidade de aprendizado contínuo.

---

**Desenvolvido com 💼 por Higor Francisco Fulaneti Barreto**
