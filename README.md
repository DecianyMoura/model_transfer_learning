# Classificação de Gatos e Cachorros com Transfer Learning

Este projeto utiliza **Transfer Learning** com o modelo pré-treinado **MobileNetV2** para classificar imagens de **gatos e cachorros**. O notebook foi desenvolvido no **Google Colab** e utiliza o dataset `cats_vs_dogs` do **TensorFlow Datasets**.

---

Dataset

- O dataset utilizado é o **Cats vs Dogs**, disponível no TensorFlow Datasets: [Link do dataset](https://www.tensorflow.org/datasets/catalog/cats_vs_dogs).  
- O conjunto é dividido em **treino** e **validação**:
  - Treino: 80% das imagens  
  - Validação: 20% das imagens  

> Obs.: Para fins de treinamento rápido, no notebook foi utilizado um **subset menor** do dataset.

---

## Tecnologias

- Python 3.x  
- TensorFlow 2.x  
- TensorFlow Datasets  
- Keras  
- Matplotlib  

---

## Como usar

1. Abra o notebook no **Google Colab**.  
2. Execute as células na ordem:
   1. Importação das bibliotecas  
   2. Carregamento do dataset  
   3. Pré-processamento das imagens  
   4. Construção e treino do modelo  
   5. Função `testar_imagem()` para upload e predição  

3. Para testar suas imagens, faça upload usando a célula de teste:  

```python
from google.colab import files

uploaded = files.upload()
for nome_arquivo in uploaded.keys():
    testar_imagem(nome_arquivo)

