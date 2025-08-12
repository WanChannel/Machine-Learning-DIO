Bibliotecas utilizadas
1. <n> Tensorflow </n>
- Principal framework para criação e treinamento de redes neurais.

- Especificamente:

  - tensorflow.keras.datasets: Para carregar o dataset MNIST.

  - tensorflow.keras.layers: Para definir camadas da rede neural.

  - tensorflow.keras.models: Para construir o modelo da rede.

  - tensorflow.keras.utils.to_categorical: Para converter rótulos em codificação one-hot.

 2. <n> sklearn.metrics </n>
 

- Ferramentas para avaliação de modelos:

  - roc_curve: Para calcular a curva ROC.

  - auc: Para calcular a área sob a curva ROC.

  - confusion_matrix: Para calcular matriz de confusão.

3. <n> matplotlib.pyplot </n>

   - Biblioteca para criação de gráficos, usada para plotar curvas ROC, matrizes de confusão, etc.

4. <n> numpy </n>

   - Biblioteca para manipulação numérica, arrays, normalização e preparação dos dados.

5. <n> seaborn </n>

   - Biblioteca para visualização estatística, usada para plotar matrizes de confusão com uma estética melhor.

6. <n> pandas </n>

   - Biblioteca para manipulação e análise de dados (embora não tenha aparecido no trecho inicial, está importada, provavelmente para manipulação tabular).


Funcionalidades implementadas no código
- Carregamento do dataset MNIST

- Base de imagens de dígitos manuscritos (28x28 pixels) usada para treinamento e teste.

- Pré-processamento das imagens

- Conversão dos pixels para float32 e normalização dividindo por 255.

- Expansão da dimensão das imagens para adicionar o canal único (escala de cinza).

- Pré-processamento dos rótulos

- Conversão dos labels para one-hot encoding com 10 classes (dígitos 0-9).

- Construção e treinamento de uma CNN (Convolutional Neural Network)

- Usando camadas convolucionais, pooling, flatten, dense.

- Modelo treinado para classificar dígitos.

- Avaliação do modelo

- Geração de matriz de confusão para medir performance.

- Cálculo das métricas: recall, precisão, F-score, acurácia, especificidade.

- Plotagem da curva ROC e cálculo da área sob a curva (AUC).

- Visualização dos resultados

- Gráficos da matriz de confusão usando seaborn.

- Gráficos da curva ROC usando matplotlib.

