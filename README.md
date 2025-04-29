# FIAP - Faculdade de Informática e Administração Paulista

<p align="center">
<a href= "https://www.fiap.com.br/"><img src="assets/logo-fiap.png" alt="FIAP - Faculdade de Informática e Admnistração Paulista" border="0" width=40% height=40%></a>
</p>

<br>

# Enterprise Challenge - Sprint 2

## Beginner Coders

## 👨‍🎓 Integrantes: 
- <a href="https://www.linkedin.com/in/luana-porto-pereira-gomes/">Luana Porto Pereira Gomes</a>
- <a href="https://www.linkedin.com/in/luma-x">Luma Oliveira</a>
- <a href="https://www.linkedin.com/in/priscilla-oliveira-023007333/">Priscilla Oliveira </a>
- <a href="https://www.linkedin.com/in/paulobernardesqs?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=ios_app">Paulo Bernardes</a>  

## 👩‍🏫 Professores:
### Tutor(a) 
- <a href="https://www.linkedin.com/in/leonardoorabona/">Leonardo Ruiz</a>
### Coordenador(a)
- <a href="https://www.linkedin.com/in/profandregodoi/">André Godoi</a>


## 📜 Descrição

Este projeto tem como objetivo usar Inteligência Artificial para ajudar a prever a produtividade agrícola da soja em fazendas do Mato Grosso.

## 📝 Sobre o Projeto
Foram utilizados dois tipos de dados:
- **NDVI (índice de vegetação)** obtido do sistema SATVeg da Embrapa.
- **Produtividade agrícola (rendimento médio)** obtido do sistema IBGE/SIDRA.
O trabalho foi desenvolvido como parte da Sprint 2 do Enterprise Challenge da 
FIAP, no 2º semestre do curso de Inteligência Artificial.

## 📁 Estrutura de pastas

Dentre os arquivos e pastas presentes na raiz do projeto, definem-se:

- <b>assets</b>: aqui estão os arquivos relacionados a elementos não-estruturados deste repositório, como imagens.

- <b>dados</b>: aqui estão os dados utilizados no notebook.
  
- <b>notebook</b>: aqui está o download do notebook em .ipynb.

- <b>README.md</b>: arquivo que serve como guia e explicação geral sobre o projeto (o mesmo que você está lendo agora).

## 🔧 Como executar o código
### 🐍 Código Python:
   - Executar por meio do link do notebook: https://colab.research.google.com/drive/1icOkQigR_feW98v80oaix2Rn1Lwb-yil?usp=sharing#scrollTo=QSR7hEkQUob0
   - Faça upload dos arquivos de dados (.xlsx).
   - Execute as células do notebook em sequência.


## 🎥 Link do vídeo: ...

## ⚙️ Etapas Realizadas
**1. Coleta e Organização dos Dados:**
- Baixamos séries históricas de NDVI de áreas agrícolas usando o SATVeg.
- Coletamos dados oficiais de produtividade da soja no IBGE/SIDRA.
- Juntamos as informações em planilhas para análise.
  
**2. Análise Exploratória:**
- Fizemos gráficos para ver o comportamento do NDVI ao longo dos anos.
- Analisamos se existia relação entre o NDVI e a produtividade da soja.
  
**3. Modelagem de Regressão:**
- Aplicamos os modelos KNN, Random Forest e SVM para prever o valor da 
produtividade (em kg/ha).
- Avaliamos os modelos usando R² e MAE.
  
**4. Modelagem de Classificação:**
- Classificamos a produtividade como "Boa" ou "Má" com base no NDVI médio.
- Aplicamos Random Forest, KNN e SVM para prever a categoria.
- Avaliamos os modelos usando a acurácia.

## 📊 Principais Resultados
### Modelagem de Regressão:
| Modelo | R² | MAE (kg/ha) |
|:-------|:--|:------------|
| SVM Regressor | -0.0430 | 121.54 |
| KNN Regressor | -0.2111 | 141.61 |
| Random Forest Regressor | -1.1485 | 187.17 |
- Melhor resultado de regressão: **SVM Regressor** (menor MAE).
### Modelagem de Classificação:
| Modelo | Acurácia |
|:-------|:---------|
| Random Forest Classifier | 1.0000 |
| KNN Classifier | 0.8333 |
| SVM Classifier | 0.8333 |
- Melhor resultado de classificação: **Random Forest Classifier** (acurácia 
100%).
  
## 🧠 Conclusão
Mesmo usando apenas o NDVI, conseguimos montar modelos que tiveram bons 
resultados de classificação e resultados razoáveis de regressão.
Os dados mostraram que o NDVI pode ser um bom começo para prever a 
produtividade agrícola, mas para melhorar a previsão seria importante usar 
também informações de clima, solo e manejo.

## 🛠️ Tecnologias Utilizadas
- Python 3.11
- Google Colab
- Pandas
- Scikit-learn
- Matplotlib
- SATVeg (Embrapa)
- IBGE/SIDRA


## 🗃 Histórico de lançamentos

* 0.5.0 - XX/XX/2024
    * 
* 0.4.0 - XX/XX/2024
    * 
* 0.3.0 - XX/XX/2024
    * 
* 0.2.0 - XX/XX/2024
    * 
* 0.1.0 - XX/XX/2024
    *

## 📋 Licença

<img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/cc.svg?ref=chooser-v1"><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/by.svg?ref=chooser-v1"><p xmlns:cc="http://creativecommons.org/ns#" xmlns:dct="http://purl.org/dc/terms/"><a property="dct:title" rel="cc:attributionURL" href="https://github.com/agodoi/template">MODELO GIT FIAP</a> por <a rel="cc:attributionURL dct:creator" property="cc:attributionName" href="https://fiap.com.br">Fiap</a> está licenciado sobre <a href="http://creativecommons.org/licenses/by/4.0/?ref=chooser-v1" target="_blank" rel="license noopener noreferrer" style="display:inline-block;">Attribution 4.0 International</a>.</p>
