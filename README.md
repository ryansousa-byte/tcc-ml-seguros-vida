# Uso de Aprendizado de Máquina para Previsão de Riscos em Seguros de Vida

Este repositório contém o código, experimentos, dados processados e documentação utilizados no Trabalho de Conclusão de Curso (TCC) **"Uso de Aprendizado de Máquina para Previsão de Riscos em Seguros de Vida: Uma Análise das Aplicações e Impactos no Mercado Securitário Brasileiro"**.

O objetivo principal deste projeto é investigar a aplicação de técnicas de Machine Learning para previsão de risco em seguros de vida, explorando impacto, viabilidade e desempenho de diferentes modelos supervisionados.

---

## 🗂 Estrutura do Repositório

/tcc-ml-seguros-vida
│
├── data/ # Arquivos de dados originais ou tratados
├── notebooks/ # Notebooks Jupyter usados nos testes
├── src/ # Código-fonte dos modelos e pipelines
├── models/ # Modelos treinados (salvos em .pkl)
├── results/ # Tabelas, métricas e gráficos gerados
├── images/ # Imagens de trechos de código citadas no TCC
├── README.md # Documentação principal do projeto
└── requirements.txt # Lista de dependências do projeto

pgsql
Copiar código

> Obs.: As pastas serão criadas automaticamente quando você subir os arquivos; caso não existam, pode criá-las manualmente.

---

## 📌 Tecnologias e Bibliotecas Utilizadas

```python
import pandas as pd
import numpy as np

from sklearn.model_selection import train_test_split
from sklearn.preprocessing import StandardScaler, OneHotEncoder
from sklearn.impute import SimpleImputer
from sklearn.metrics import accuracy_score, classification_report, confusion_matrix
from sklearn.ensemble import RandomForestClassifier

import xgboost as xgb
from imblearn.over_sampling import SMOTE
🧪 Experimentos Realizados
O projeto avaliou diferentes abordagens para previsão de risco:

✔ Modelo 1 — LGBM otimizado para equilíbrio entre precisão e recall
Métrica: f1_macro

Técnica: Optuna (50 iterações)

Resultado: 0,70 de acurácia média

✔ Modelo 2 — LGBM focado na acurácia
Parâmetros finais ajustados para maior acurácia

Resultado:

Acurácia: 0,792

Precisão: 0,80

Recall ponderado: 0,79

✔ Modelo 3 — Pipeline completo + Random Forest
Normalização

One-hot encoding

Feature engineering

SMOTE (balanceamento)

Resultado:

Acurácia: 0,792

Precisão: 0,80

Recall: 0,79

🖼 Imagens de Código Citadas no TCC
Coloque aqui as imagens contendo trechos relevantes do código, como:

Pipeline de pré-processamento

Configuração dos modelos

Otimização com Optuna

Aplicação do SMOTE

Treinamento final dos modelos

Exemplo:

bash
Copiar código
/images/optuna_tuning.png
/images/random_forest_pipeline.png
No TCC, basta referenciar assim:

“Conforme apresentado na Figura X disponível no repositório GitHub (pasta /images), o pipeline de pré-processamento utilizou padronização numérica e codificação one-hot.”

▶ Como Executar o Projeto
1. Clone o repositório
bash
Copiar código
git clone https://github.com/seu-usuario/tcc-ml-seguros-vida.git
cd tcc-ml-seguros-vida
2. Instale as dependências
Crie um ambiente virtual opcionalmente, depois:

bash
Copiar código
pip install -r requirements.txt
3. Execute os notebooks
Abra os arquivos da pasta /notebooks para replicar os experimentos.

📄 requirements.txt (sugestão completa)
txt
Copiar código
pandas
numpy
scikit-learn
xgboost
imbalanced-learn
matplotlib
seaborn
optuna
📚 Finalidade Acadêmica
Este repositório faz parte do TCC do curso de Sistemas de Informação, e tem como objetivo garantir reprodutibilidade, transparência e documentação completa dos experimentos relacionados ao uso de Machine Learning para previsão de risco em seguros de vida.

📬 Contato
Caso queira entrar em contato sobre o projeto:

Autor: Ryan Paulo
Projeto acadêmico — 2025
