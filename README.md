# 🍦 Projeto Gelato Mágico: Previsão de Vendas com Azure AI

![Logo da Gelato Mágico](logo.png)

## 📖 A História da Gelato Mágico
A **Gelato Mágico** nasceu do sonho da Dona Magali em trazer o verdadeiro gelato artesanal para o coração de **Varginha, MG**. O negócio cresceu, mas surgiu um desafio: como prever a quantidade de sorvete a ser produzida para evitar desperdícios em dias frios ou falta de estoque em dias de calor intenso? Este projeto utiliza Inteligência Artificial para transformar a temperatura local em previsões precisas de vendas.

---

## 🛠️ Tecnologias e Ferramentas
* **Cloud Computing**: Microsoft Azure
* **IA Service**: Azure Machine Learning (Automated ML)
* **Algoritmo**: Regressão Linear e VotingEnsemble
* **Dados**: Dataset Tabular (CSV)

---

## 📊 Ciclo de Desenvolvimento na Azure

### 1. Ingestão e Tratamento de Dados
Os dados foram importados como um **Ativo de Dados Tabular**. Foi necessário ajustar o delimitador para **ponto e vírgula** para que o Azure reconhecesse as colunas de `data`, `temperatura_max` e `vendas_sorvete` corretamente.

![Preparação de Dados](screenshots/preparacao_de_dados.png)

### 2. Configuração da Arquitetura (Designer)
Utilizei o Azure ML Designer para criar um fluxo lógico de treinamento, incluindo a separação de dados (Split Data) e a aplicação do algoritmo de Regressão Linear.

![Arquitetura do Modelo](screenshots/Arquitetura_do_Modelo.png)

### 3. Treinamento Automatizado (AutoML)
O experimento foi configurado para uma tarefa de **Regressão**, com um limite de tempo de 15 minutos para otimização de custos e proteção dos créditos de estudante. O status final do trabalho foi **Concluído**.

![Status do Treinamento](screenshots/Treinamento.png)

### 4. Análise do Melhor Modelo
O Azure identificou o algoritmo **VotingEnsemble** como o mais eficiente, apresentando um erro quadrático médio de apenas **0.12153**, garantindo alta fidelidade nas previsões.

![Resultados Finais](screenshots/Resultados_Finais.png)

---

## 📈 Impacto no Negócio
Com este modelo implementado, a Dona Magali consegue agora:
1. **Reduzir o desperdício** de matéria-prima em até 20%.
2. **Garantir o estoque** nos dias de pico de calor em Varginha.
3. **Planejar escalas de trabalho** (RH) baseadas na demanda prevista.

---

## 👩‍💻 Autora
**Jéssica**
Estudante de Sistemas de Desenvolvimento no IFSULDEMINAS e Profissional de RH.
