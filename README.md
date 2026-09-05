# Tarefa 3 – CNNs para reconhecimento de caracteres

## Objetivo

Nesta tarefa foram desenvolvidas três redes neurais convolucionais (CNNs), baseadas nas arquiteturas apresentadas no trabalho de Silva Filho et al., para o reconhecimento de:

- Dígitos: 1, 2, 3, 4 e 5;
- Letras: A, B, C, D e E;
- Respostas: V e F.

Foram utilizados subconjuntos da base **EMNIST**, e os modelos foram desenvolvidos utilizando **TensorFlow/Keras**.

## Resultados

Os modelos apresentaram os seguintes resultados no conjunto de teste:

| Modelo | Acurácia | Parâmetros treináveis | Tamanho (.keras) |
|---|---:|---:|---:|
| Dígitos | **99,71%** | 69.477 | 0,845 MB |
| Letras | **99,19%** | 69.477 | 0,845 MB |
| V/F | **99,96%** | 65.122 | 0,789 MB |

Após o treinamento, os três modelos foram exportados no formato `.keras`.

## Redução do tamanho dos modelos

Também foi realizada a conversão dos modelos para **TensorFlow Lite (TFLite) com otimização**, permitindo reduzir significativamente o tamanho dos arquivos.

| Modelo | Keras (MB) | TFLite (MB) | Redução |
|---|---:|---:|---:|
| Dígitos | 0,845287 | 0,076401 | **90,96%** |
| Letras | 0,845299 | 0,076431 | **90,96%** |
| V/F | 0,788554 | 0,070221 | **91,09%** |

Os resultados mostram uma redução superior a **90%** nos três modelos, tornando-os mais leves para armazenamento e utilização.

## Tecnologias utilizadas

- Python
- TensorFlow/Keras
- EMNIST
- CNN
- TensorFlow Lite
- Google Colab

## Notebook

O código completo e as células executáveis da atividade estão disponíveis no Google Colab:

[Acessar notebook no Google Colab](https://colab.research.google.com/drive/1zUiEDO7GipqsKn4STWtQ2tAnFRBj13v2)
