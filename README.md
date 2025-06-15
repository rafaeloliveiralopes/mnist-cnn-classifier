# Projeto de Classificação MNIST usando Rede Convulacional - CNN (Fundamentos da IA - Eng. Software)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)](https://opensource.org/licenses/MIT)


Repositório contendo o projeto prático desenvolvido durante o estudo da matéria 'Fundamentos da Inteligência Artificial', do curso de Engenharia de Software. O foco está na aplicação de Redes Neurais Convolucionais (CNNs) para a tarefa de classificação de imagens de dígitos manuscritos (conjunto de dados MNIST). O código demonstra as etapas essenciais para o estudo de visão computacional, desde o carregamento e preparação dos dados até a definição da arquitetura da CNN em Keras/TensorFlow e o processo de treinamento do modelo.

## Índice
- [Visão Geral do Projeto](#visão-geral-do-projeto)
- [Tecnologias e Ferramentas Utilizadas](#tecnologias-e-ferramentas-utilizadas)
- [Etapas do Desenvolvimento](#etapas-do-desenvolvimento)
- [Resultados](#resultados)
- [Como Executar o Projeto](#como-executar-o-projeto)
- [Aprendizados](#aprendizados)
- [Melhorias](#melhorias)
- [Conclusão](#conclusão)
- [Contato](#contato)

## Visão Geral do Projeto
Este projeto apresenta um pipeline completo de Machine Learning para classificação de imagens:

- Carregamento e pré-processamento de dados.
- Construção de uma CNN com camadas convolucionais, pooling e fully connected.
- Treinamento com validação em tempo real.
- Avaliação de desempenho em conjunto de teste.
- Visualização gráfica da evolução da acurácia e da perda.
- Predição de exemplos reais do dataset.

## Tecnologias e Ferramentas Utilizadas

[![Python](https://img.shields.io/badge/-Python-blue?style=for-the-badge&logo=python)](https://www.python.org/)
[![TensorFlow](https://img.shields.io/badge/-TensorFlow-orange?style=for-the-badge&logo=tensorflow)](https://www.tensorflow.org/)
[![Keras](https://img.shields.io/badge/-Keras-red?style=for-the-badge&logo=keras)](https://keras.io/)
[![Google Colab](https://img.shields.io/badge/-Google%20Colab-yellow?style=for-the-badge&logo=google-colab)](https://colab.research.google.com/)
[![Dataset MNIST](https://img.shields.io/badge/Dataset-MNIST-blueviolet?style=for-the-badge)](http://yann.lecun.com/exdb/mnist/)
[![Model Type CNN](https://img.shields.io/badge/Model%20Type-CNN-brightgreen?style=for-the-badge)](https://en.wikipedia.org/wiki/Convolutional_neural_network)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)](https://opensource.org/licenses/MIT)

## Etapas do Desenvolvimento

1. Processamento da imagem;
2. Preparação dos dados
3. Construção do modelo;
4. Treinamento do modelo;
5. Inferência do modelo.


## Resultados

O treinamento foi realizado utilizando 10 épocas (imagem 1). 
![Captura de tela de 2025-06-15 06-11-18](https://github.com/user-attachments/assets/1f44ce2f-c85c-4cfd-a8e5-0b9a50f3221a) Imagem 1


No entanto, conforme pode ser visualizados na imagem 2, nas primeiras épocas (0 a 2) a acurácia de treinamento começa baixa (cerca de 0.93) e sobe rapidamente. A acurácia de validação começa alta (por volta de 0.98), demonstrando que o modelo aprende rapidamente nos primeiros ciclos.

![Captura de tela de 2025-06-15 07-12-41](https://github.com/user-attachments/assets/3dd2f254-082c-49bf-bd5e-56bb7fb48513) Imagem 2


Nas épocas 3 a 5 a acurácia de treinamento continua subindo e a acurácia de validação começa a estabilizar por volta de 0.988. No entanto, foi observado que a partir da época 6 a acurácia permanece estável, mas sem muito ganho, o que pode indicar um início de overfitting. Com isso, é possível concluir que as épocas adicionais não trouxeram grandes ganhos ao modelo, sugerindo que o treinamento poderia ser parado entre as épocas 3 e 5.


## Como Executar o Projeto

Você pode rodar o projeto localmente ou no Google Colab.

### No Google Colab:

1. Faça upload do notebook: `number_recognition.ipynb`.
2. Instale as dependências caso necessário:

```python
!pip install tensorflow keras matplotlib numpy
```
3. Execute célula por célula


## Aprendizados

Este projeto reforçou mais os meus  conhecimentos no uso das principais tecnologias utilizadas para o treinamento em visão computacional. Apesar de ser um projeto simples, foi aplicada técnincas de normalização dos dados do dataset MNIST (dígitos manuscritos) divididas em treino (60.000) e teste (10.000), conversão de rótulos para one-hot encoding, aplicação das camadas Conv2D,MaxPooling2D, Flatten e Dense e plotagem dos gráficos de performance utilizando o matplotlib.

Foi aprendido que o uso do float32 no processo de normalização dos dados ao em vez do float64, se tornou o padrão, por ser observadolevando em conta eficiência de memória, velocidade computacional, precisão sufciente para treinamento para a maioria do treinamento de machine learning e compatibilidade com hardwares e bibliotecas.

## Melhorias

Que melhorias você fez no seu código? Ex: refatorações, melhorias de performance, acessibilidade, etc

## Conclusão

## Contato
🔹 **Autor:** Rafael Oliveira Lopes  
🔹 **Email:** rafaellopes.dev@email.com  
🔹 **LinkedIn:** [LinkedIn](https://www.linkedin.com/in/rafael-lopes-desenvolvedor-fullstack/)  
🔹 **Site:** [rafaellopes.dev](https://rafaellopes.dev)  
