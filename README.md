# 📌 PBL Fase 6 – Visão Computacional com YOLO e CNN

## 👨‍💻 Integrante

* Nome: *Bruno Nogueira Burian*
* RM: *568025*

---

## 📖 Sobre o Projeto

Este projeto tem como objetivo aplicar técnicas de **Visão Computacional** utilizando diferentes abordagens de redes neurais, com foco na detecção e classificação de objetos.

Foram exploradas três soluções principais:

* YOLO customizado (treinado com dataset próprio)
* YOLO pré-treinado (modelo padrão)
* CNN treinada do zero (classificação de imagens)

---

## 🧠 Tecnologias Utilizadas

* Python
* Google Colab
* YOLOv5
* TensorFlow / Keras
* Make Sense AI (rotulação)

---

## 📂 Dataset

O dataset foi construído manualmente contendo duas classes:

* 🍌 Banana
* 🎤 Microfone

Total de imagens: **80**

Divisão:

* Treino: 64 imagens
* Validação: 8 imagens
* Teste: 8 imagens

---

## 🚀 Entrega 1 – YOLO Customizado

Foi realizado o treinamento de um modelo YOLOv5 com dataset próprio.

### 🔹 Resultados (30 épocas)

* mAP50: ~0.16
* Recall: ~0.13
* Precision: ~0.12

### 🔹 Resultados (60 épocas)

* mAP50: ~0.17
* Recall: ~0.25
* Precision: ~0.08

### 📌 Conclusão

O aumento de épocas trouxe leve melhora no recall, porém reduziu a precisão, indicando possível **overfitting**.

---

## 🔍 Entrega 2 – Comparação de Abordagens

### 🔹 YOLO Pré-treinado

* Funcionou bem para **banana** (classe conhecida)
* Falhou para **microfone**
* Em alguns casos classificou como objetos incorretos (ex: toothbrush)

📌 Conclusão:
Modelo eficiente apenas para classes já conhecidas.

---

### 🔹 CNN (Classificação)

* Acurácia de treino: ~100%
* Acurácia de validação: ~87% a 100%

📌 Conclusão:
Alta performance na classificação, porém não realiza detecção de objetos.

---

## 📊 Comparação Final

| Critério    | YOLO Custom | YOLO Padrão  | CNN           |
| ----------- | ----------- | ------------ | ------------- |
| Tipo        | Detecção    | Detecção     | Classificação |
| Facilidade  | Média       | Alta         | Média         |
| Precisão    | Média/Baixa | Baixa        | Alta          |
| Treinamento | Alto        | Nenhum       | Médio         |
| Inferência  | Rápida      | Muito rápida | Rápida        |

---

## 🧾 Conclusão

Cada abordagem apresentou vantagens específicas:

* YOLO Custom → melhor para detecção de objetos específicos
* YOLO Padrão → rápido, mas limitado a classes conhecidas
* CNN → excelente para classificação, mas não detecta objetos

A escolha do modelo depende diretamente do problema a ser resolvido.

---

## 📎 Notebook

🔗 *Cole aqui o link do seu Colab/Jupyter*

---

## ⚙️ Considerações Finais

Possíveis melhorias:

* Aumentar o dataset
* Melhorar rotulação
* Ajustar hiperparâmetros
* Utilizar GPU para treinamento

---
