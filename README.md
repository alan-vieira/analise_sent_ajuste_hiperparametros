# ⚙️ Otimização de Modelos: Fine-tuning via GridSearchCV

## 📖 Descrição

Este repositório documenta a etapa de refinamento dos modelos de Machine Learning pré-selecionados. Após identificar os melhores algoritmos na fase de treinamento, utilizei a técnica de **Grid Search com Cross-Validation** para encontrar a combinação ideal de hiperparâmetros, visando a redução do overfitting e o aumento da acurácia final.

## 🧪 Estrutura da Otimização

A busca pelos melhores parâmetros foi realizada em dois cenários críticos para garantir a consistência dos resultados:

1. [Ajuste com Oversampling](https://github.com/alan-vieira/analise_sent_ajuste_hiperparametros/blob/main/ajuste_hiperparametros_over.ipynb): Otimização focada no modelo treinado com dados superamostrados, buscando o equilíbrio entre as classes.

2. [Ajuste com Undersampling](https://github.com/alan-vieira/analise_sent_ajuste_hiperparametros/blob/main/ajuste_hiperparametros_under.ipynb): Refinamento do modelo baseado em dados sobamostrados, priorizando a precisão em um conjunto de dados mais enxuto.

## 🛠️ O que foi otimizado?

Através do GridSearchCV, foram testados diferentes valores para:

- **Parâmetros de Regularização (C, Alpha)**: Para controlar a complexidade do modelo.

- **Critérios de Divisão e Profundidade**: No caso de modelos baseados em árvores.

- **Kernels e Penalidades**: Dependendo do algoritmo selecionado (Logistic Regression, SVM, etc.).

## 📊 Resultados Esperados

O output deste processo é o modelo "campeão" salvo (geralmente via `joblib` ou `pickle`), pronto para ser consumido pela API de produção. A otimização garantiu um ganho incremental de performance que faz a diferença em ambientes de tempo real (Twitter).

## 🚀 Como Executar

1. Clone o repositório.

2. Certifique-se de ter os arquivos de dados (ou modelos base) conforme estruturado nos notebooks.

3. Instale o Scikit-Learn: pip install scikit-learn.

## 📺 Demonstração

Acompanhe a explicação técnica detalhada no YouTube:

🔗 [Assistir vídeo explicativo](https://www.youtube.com/watch?v=K7BGt9F1mZo)

## 👤 Autor

**Alan Vieira** - *Engenheiro de Telecomunicações & Especialista em Dados*

- [LinkedIn](https://www.linkedin.com/in/alansilvavieira)

- [GitHub Portfólio](https://github.com/alan-vieira)
