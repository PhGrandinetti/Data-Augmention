# # 📊 Projeto de Data Augmentation em Visão Computacional

## 📌 Descrição

Este projeto tem como objetivo aplicar técnicas de **Data Augmentation** em imagens, utilizando transformações geométricas e ajustes de iluminação.

Foram desenvolvidas duas etapas principais:

- **Exercício 1:** Geração automática de um dataset aumentado.
- **Exercício 2:** Interface gráfica interativa para visualização das transformações.

---

# 🧪 Exercício 1 — Geração de Dataset Aumentado

## 🎯 Objetivo

Gerar múltiplas variações de uma imagem original utilizando transformações aleatórias.

---

## ⚙️ Transformações aplicadas

Cada imagem gerada sofre combinações aleatórias das seguintes transformações:

- 🔄 Rotação (−30° a +30°)
- 📏 Escala (0.8x a 1.2x)
- ↔️ Translação (até ±50 pixels)
- 🔁 Flip horizontal (50% de chance)
- 🌗 Ajuste de gamma (0.7 a 1.3)

---

## 📂 Saída

- 30 imagens geradas automaticamente
- Salvas na pasta:
- dataset_aumentado/
- Nomeadas como:
- aug_001.png, aug_002.png, ..., aug_030.png

  
---

## 📊 Estatísticas exibidas

Durante a execução, o script mostra:

- Média, mínimo e máximo das rotações
- Média, mínimo e máximo das escalas
- Média, mínimo e máximo do gamma
- Quantidade de imagens com flip

---

## 🖼️ Exemplo de resultados

<img width="982" height="789" alt="image" src="https://github.com/user-attachments/assets/e6f311ae-d344-415a-bccf-8b7e6005075d" />


---

## ▶️ Como executar

Este exercício foi desenvolvido para ser executado no **Google Colab**.

### 📌 Passos:

1. Acesse o arquivo:
  - `exercicio-01-paulo.ipynb`

2. Faça upload da imagem que será utilizada e/ou ajuste o caminho da imagem no código.

3. Execute todas as células do notebook:
   - Menu: **Ambiente de execução → Executar tudo**
   - Ou use: `Ctrl + F9`

4. O código irá:
   - Gerar automaticamente 30 variações da imagem
   - Salvar na pasta:
     ```
     dataset_aumentado/
     ```
   - Exibir estatísticas no terminal
   - Mostrar uma grade com exemplos gerados

---

### ⚠️ Observação

Se estiver utilizando o Google Drive, certifique-se de montar o drive corretamente:


from google.colab import drive
drive.mount('/content/drive')

# 🎨 Exercício 2 — Interface Interativa

## 🎯 Objetivo

Criar uma interface gráfica para visualizar, em tempo real, transformações de data augmentation em imagens.

---

## 📁 Arquivo principal

- `exercicio-02-paulo.ipynb`

---

## 🖥️ Funcionalidades

- Upload de imagem
- Ajuste de parâmetros via sliders:
  - 🔄 Rotação
  - 📏 Escala
  - ↔️ Translação (X e Y)
  - 🌗 Gamma
- 🔁 Checkbox para flip horizontal
- 🖼️ Visualização lado a lado:
  - Imagem original
  - Imagem transformada

---

## ⚙️ Funcionamento

A interface foi construída utilizando a biblioteca Gradio, permitindo interação direta com os parâmetros.

A cada alteração nos sliders ou checkbox, a imagem transformada é atualizada automaticamente, possibilitando uma análise visual imediata das transformações aplicadas.

---

## 🖼️ Exemplo da interface

<img width="1181" height="906" alt="image" src="https://github.com/user-attachments/assets/042ce831-54ba-471d-b085-4dbdad8c9c5d" />


---

## ▶️ Como executar

Este exercício foi desenvolvido para ser executado no **Google Colab**.

### 📌 Passos:

1. Acesse o arquivo:
   - `exercicio-02-paulo.ipynb`
2. Execute todas as células:
   - Menu: **Ambiente de execução → Executar tudo**
   - Ou use: `Ctrl + F9`

3. Após a execução, o Colab irá gerar um link público do Gradio.

4. Clique no link para abrir a interface interativa no navegador.

---

### ⚠️ Observação

Ao executar no Colab, o Gradio pode exibir uma mensagem como:
  Running on public URL...
Isso é esperado — significa que a interface está disponível temporariamente online.

---

# 🧰 Tecnologias Utilizadas

- **Python** → Linguagem principal do projeto  
- **OpenCV (cv2)** → Processamento e transformação de imagens  
- **NumPy** → Manipulação de arrays e geração de valores aleatórios  
- **Matplotlib** → Visualização de imagens (Exercício 1)  
- **Gradio** → Criação da interface gráfica interativa (Exercício 2)  
- **Google Colab** → Ambiente de execução dos notebooks  

---

# 📚 Conceitos Abordados

## 🎯 Data Augmentation
Técnica utilizada para gerar novas variações de imagens a partir de uma imagem original, aumentando a diversidade dos dados.

---

## 🔄 Transformações Geométricas
Aplicação de operações espaciais na imagem:
- Rotação
- Escala
- Translação
- Reflexão (flip)

---

## 🌗 Ajuste de Iluminação (Gamma)
Transformação que altera o brilho e contraste da imagem através da correção de gamma.

---

## 🎲 Aleatoriedade Controlada
Uso de geração de números aleatórios para criar variações diferentes de forma controlada, utilizando `NumPy`.

---

## 🖼️ Processamento de Imagens
Manipulação direta dos pixels da imagem utilizando operações matemáticas e funções do OpenCV.

---

## 🧩 Interfaces Interativas
Criação de interfaces gráficas para interação em tempo real com parâmetros, utilizando a biblioteca Gradio.

---

## ⚙️ Automação de Geração de Dados
Criação automática de múltiplas imagens com diferentes transformações, simulando cenários reais de treinamento de modelos.

---

## ✅ Conclusão

A interface permite explorar de forma intuitiva como diferentes transformações afetam uma imagem, sendo útil tanto para aprendizado quanto para prototipação de técnicas de aumento de dados.

---
