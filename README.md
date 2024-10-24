# Projeto Rusty Bargain: Avaliação de Carros Usados

## Visão Geral
Construir e identificar o melhor modelo preditivo para determinar o valor de mercado dos veículos usados, utilizando dados históricos, especificações técnicas e versões de acabamento, com o intuito de atrair novos clientes para o aplicativo da **Rusty Bargain** (Empresa fictícia).

## Objetivos
- **Qualidade da predição**: Assegurar que os valores previstos sejam precisos.
- **Velocidade da predição**: Minimizar o tempo necessário para realizar previsões.
- **Tempo necessário para o treinamento**: Garantir que o treinamento do modelo seja eficiente.

## Ferramentas e Bibliotecas Utilizadas
- **Python**: Linguagem principal utilizada para a análise e modelagem.
- **Pandas**: Biblioteca para manipulação e análise de dados.
- **NumPy**: Biblioteca para computação numérica e manipulação de arrays.
- **Scikit-Learn**: Biblioteca para implementação de algoritmos de aprendizado de máquina.
- **LightGBM**: Biblioteca para criação de modelos de Gradient Boosting.
- **Matplotlib** e **Seaborn**: Bibliotecas para visualização de dados.

## Descrição dos Dados
O conjunto de dados `car_data.csv` contém as seguintes características:

- **DateCrawled**: Data em que o perfil foi baixado do banco de dados.
- **VehicleType**: Tipo de carroçaria do veículo.
- **RegistrationYear**: Ano de matrícula do veículo.
- **Gearbox**: Tipo de caixa de transmissão.
- **Power**: Potência (hp).
- **Model**: Modelo do veículo.
- **Mileage**: Quilometragem (medida em km).
- **RegistrationMonth**: Mês de registro do veículo.
- **FuelType**: Tipo de combustível.
- **Brand**: Marca do veículo.
- **NotRepaired**: Indica se o veículo foi reparado ou não.
- **DateCreated**: Data de criação do perfil.
- **NumberOfPictures**: Número de fotos do veículo.
- **PostalCode**: Código postal do proprietário do perfil.
- **LastSeen**: Data da última atividade do usuário.

**Objetivo**:
- **Price**: Preço do veículo em Euros.

## Instruções do Projeto
1. **Carregamento dos Dados**:
   - Importação do conjunto de dados a partir do arquivo `car_data.csv`.

2. **Verificação da Qualidade dos Dados**:
   - Análise dos dados para garantir que não há valores ausentes ou extremos.
   - Aplicação de limpeza e pré-processamento conforme necessário.

3. **Tarefa 1 - Treinamento de Modelos**:
   - Treinamento de diferentes modelos, incluindo Regressão Linear, Árvore de Decisão e Floresta Aleatória, para prever o preço dos veículos.

4. **Tarefa 2 - Implementação do Gradient Boosting**:
   - Utilização da biblioteca LightGBM para criar um modelo de Gradient Boosting com ajuste de hiperparâmetros.

5. **Avaliação de Modelos**:
   - Cálculo da métrica REQM para comparar a qualidade das previsões entre os modelos treinados.

6. **Análise de Desempenho**:
   - Medição do tempo de execução para cada modelo e comparação da eficiência computacional, especialmente entre LightGBM e Floresta Aleatória.

7. **Relatório de Resultados**:
   - Compilação e análise dos resultados obtidos, incluindo as previsões e a performance de cada modelo.

## Conclusão
O objetivo deste projeto foi desenvolver um modelo de aprendizado de máquina para prever o valor de mercado de carros usados, utilizando uma abordagem de regressão. Foram testados diferentes modelos, incluindo Regressão Linear, Árvore de Decisão, Floresta Aleatória, Gradient Boosting e LightGBM, com ajuste de hiperparâmetros para otimizar o desempenho.

### Análise dos Resultados
- **Melhor Modelo**: LightGBM
  - O modelo LightGBM apresentou o menor REQM (1536.37) nos dados de teste, com um tempo de execução eficiente. Comparado com a Floresta Aleatória e Gradient Boosting, o LightGBM teve um desempenho ligeiramente superior, tornando-se a escolha ideal para implementação final.
  
- **Desempenho vs. Tempo**:
  - O tempo de execução do LightGBM foi significativamente menor que o da Floresta Aleatória, refletindo a eficiência do modelo em termos de tempo e recursos computacionais. Se a velocidade for mais importante que a precisão, o uso do Gradient Boosting pode ser reconsiderado.

## Aprendizados
Este projeto permitiu-me desenvolver as seguintes habilidades:
- **Análise de Dados**: Aprendi a manipular e explorar conjuntos de dados para obter insights significativos.
- **Modelagem Preditiva**: Aprofundei meus conhecimentos em diversas técnicas de aprendizado de máquina, incluindo regressão linear e métodos baseados em árvore.
- **Otimização de Modelos**: Compreendi a importância do ajuste de hiperparâmetros para melhorar o desempenho dos modelos.
- **Avaliação de Modelos**: Aprendi a utilizar a métrica REQM para avaliar a eficácia das predições.
- **Eficiência Computacional**: Desenvolvi habilidades para medir e otimizar o tempo de execução dos modelos.

## Como Executar o Projeto
- Clone o repositório.
- Navegue até o diretório do projeto.
- Abra o projeto no seu IDE favorito.
- Instale as dependências.
- Execute o script principal.

## Contato

Luciano Pinto
[LinkedIn](https://www.linkedin.com/in/lucianolcp/)  
Email: dslucianopinto@gmail.com
