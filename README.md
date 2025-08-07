# TelecomX_parte2_BR
# Análise de Evasão de Clientes (Churn)

## 📋 Descrição
Este projeto tem como objetivo desenvolver modelos preditivos capazes de prever quais clientes têm maior chance de cancelar seus serviços. Atravez da modelagem e da análise de correlação e seleção de variáveis, treinamento de modelos de classificação, avaliação de desempenho dos modelos com métricas. E por fim interpretar os resultados, incluindo a importância das variáveis, é apontar os principais fatores que influenciam a evasão.


## 📂 Estrutura do Projeto

- `dados_tratados.csv`: Base de dados usada no projeto.
- `README.md`: Documento de apresentação do projeto.
- `TelecomX_Parte2_dicionario.md`: Dicionario de dados.
- `TelecomX_part2_BR.ipynb`: Notebook com todo o passo a passo da análise.

---

## 🔍 Etapas da Análise

1. **Preparação dos Dados**

2. **Correlação e Seleção de Variáveis**

3. **Modelagem Preditiva**
   
4. **Interpretação e Conclusões**
---

## 🚀 Modelos Usados e sua Justificativa

- Regressão Logística:
Fácil de interpretar e entender o impacto das variáveis. Requer dados balanceados para melhorar o desempenho, por isso usar SMOTE.
Precisa normalizar para que o modelo funcione corretamente, pois depende da escala das variáveis para otimizar os coeficientes.

- Random Forest:
Captura relações complexas e não lineares. Mais robusto a dados desbalanceados e não precisa de balanceamento para funcionar bem.
Não precisa normalizar porque baseia-se em divisões das variáveis, que não são afetadas pela escala.

## 💡 Conclusões

Os modelos de Regressão Logística (com SMOTE) e Random Forest apresentaram desempenho parecido, com acurácia em torno de 78-79%. A Regressão Logística identificou melhor os clientes que realmente evadem (recall 63%), enquanto o Random Forest teve maior precisão (64%).

As variáveis que mais influenciam a evasão são:
- Gasto mensal e gasto total: clientes que gastam mais têm maior risco de evasão.
- Tipo de contrato: contratos longos (1 ou 2 anos) reduzem a evasão; contratos mês a mês aumentam o risco.
- Tempo de contato: quanto maior o tempo com a empresa, menor a evasão.
- Tipo de internet: clientes com fibra óptica evadem menos.
- Forma de pagamento: uso de cheque eletrônico está associado a menor evasão.
- Serviços adicionais (suporte técnico, streaming, segurança) ajudam a reduzir evasão, porém com menor impacto.

Estratégias para reduzir evasão:
- Criar planos e benefícios para clientes com gastos altos.
- Incentivar contratos longos com descontos ou vantagens.
- Investir na qualidade da fibra óptica e no suporte técnico.
- Fortalecer o relacionamento com clientes, especialmente os novos.
- Facilitar e promover formas de pagamento que aumentem retenção.


## 🚀 Tecnologias Utilizadas

- Python
- NumPy
- Pandas
- Scikit-learn (sklearn)
- Imbalanced-learn (imblearn)
- Seaborn
- Matplotlib
- Google Colab

---
