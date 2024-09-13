# Desempenho de Classificadores - Análise de Dados

## Objetivo Principal

Desenvolver classificadores para o conjunto de dados "Letter Recognition" da UCI. O objetivo é identificar caracteres como uma das 26 letras maiúsculas do alfabeto inglês, utilizando diferentes técnicas de classificação. As imagens são convertidas em 16 atributos numéricos que serão usados nos classificadores.

Link para o conjunto de dados: [Letter Recognition Dataset](https://archive.ics.uci.edu/static/public/59/letter+recognition).

## Tarefas

1. **Classificador baseado na Distância de Mahalanobis**
   - Usando todos os parâmetros da base de dados.
   - Usando n parâmetros da base de dados.

2. **Classificador baseado em KNN (K-nearest neighbors)**
   - Usando todos os parâmetros da base de dados.
   - Usando n parâmetros da base de dados.

3. **Classificador baseado em LDA (Linear Discriminant Analysis)**
   - Usando todos os parâmetros da base de dados.
   - Usando n parâmetros da base de dados.

4. **Classificador baseado em Rede Neural MLP (Multilayer Perceptron)**
   - Usando todos os parâmetros da base de dados.

5. **Classificador baseado em Máquinas de Vetores de Suporte Não-Linear (SVM)**
   - Usando kernel radial (RBF) e todos os parâmetros da base de dados.

## Pré-processamento

- **Divisão dos dados:** Holdout com 70% para treino e 30% para teste.
- **Normalização:** Aplicada nos dados de treino e replicada nos dados de teste.
- **Balanceamento de Classes:** Utilização da técnica SMOTE para balancear as classes.
- **Codificação das Labels:** Transformação das classes em valores numéricos.
- **Seleção de Parâmetros:** Utilização de técnicas como correlação, informação mútua, razão discriminante de Fisher e PCA.

## Classificadores Implementados

1. **Distância de Mahalanobis**
2. **k-NN (K-nearest neighbors)**
3. **LDA (Linear Discriminant Analysis)**
4. **Rede Neural MLP (Multilayer Perceptron)**
5. **Máquinas de Vetores de Suporte (SVM com kernel radial)**

## Métricas de Desempenho

As métricas avaliadas em cada classificador são:

- **Acurácia:** Proporção de previsões corretas.
- **Sensibilidade:** Taxa de verdadeiros positivos.
- **Especificidade:** Taxa de verdadeiros negativos.

## Bibliotecas Utilizadas

- `numpy`
- `pandas`
- `matplotlib`
- `seaborn`
- `scikit-learn`
- `imblearn`
- `ucimlrepo`
- `scipy`

## Como Executar

1. Certifique-se de que o `Poetry` está instalado. Se ainda não estiver, instale com o comando:

    ```bash
    pip install poetry
    ```

2. Instale as dependências do projeto com o comando:

    ```bash
    poetry install
    ```

3. Para ativar o ambiente virtual gerenciado pelo Poetry, utilize:

    ```bash
    poetry shell
    ```

4. Execute o script principal:

    ```bash
    python main.py
    ```

O script irá carregar o conjunto de dados, realizar o pré-processamento, treinar os classificadores e exibir as métricas de desempenho para cada um.

## Contribuições

Contribuições são bem-vindas! Sinta-se à vontade para abrir uma _issue_ ou _pull request_ para melhorias.

## Licença

Este projeto é licenciado sob os termos da MIT License.
