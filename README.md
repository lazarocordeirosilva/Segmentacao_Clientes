![segmentação](https://github.com/user-attachments/assets/e2b53cc4-ff9b-40e6-962c-eb66c3ad00d4)

# Segmentação de Clientes: Análise e Clusterização 

## Segmentação de Clientes

Este projeto realiza uma análise detalhada sobre a segmentação de clientes a partir de respostas a um questionário de 30 questões. A segmentação de clientes é um processo crucial para as empresas, pois permite a identificação de padrões comportamentais e preferências de diferentes grupos, facilitando a criação de estratégias personalizadas de marketing e relacionamento. Utilizar técnicas de Machine Learning, como a redução de dimensionalidade e algoritmos de clusterização, proporciona uma visão mais clara sobre esses padrões, permitindo a tomada de decisões mais assertivas, otimizando o direcionamento de recursos e, consequentemente, melhorando a experiência do cliente e o desempenho financeiro da empresa.

## Objetivo
O objetivo deste projeto é aplicar a técnica de PCA (Análise de Componentes Principais) para reduzir a dimensionalidade dos dados gerados por um questionário de 30 questões acerca de um produto (microvan), garantindo que as informações mais relevantes sejam preservadas. Com a base de dados reduzida, utilizamos técnicas de aprendizado de máquina não supervisionado, especificamente algoritmos de clusterização (KMeans), para identificar grupos de clientes com características e comportamentos semelhantes. A segmentação gerada será utilizada como base para ações estratégicas, auxiliando a empresa a compreender melhor o perfil dos seus clientes e a implementar abordagens personalizadas de marketing e atendimento.

Essa descrição mantém a mesma abordagem clara e focada nos benefícios para a empresa, como o aumento da eficiência e da assertividade na tomada de decisões.
 
## Notebooks
O projeto está dividido em dois Notebooks: 

1. **PCA**: [PCA - Redução Dimensionalidade][https://github.com/lazarocordeirosilva/Segmentacao_Clientes/blob/main/notebook/PCA%20-%20Redu%C3%A7%C3%A3o%20Dimensionalidade.ipynb

- Neste notebook são aplicadas técnicas de redução de dimensionalidade (PCA) a fim de construir 5 componentes principais a partir de 30 features originais, referentes as respostas de um questionário acerca de um produto (microvan).

2. **Segmentação de Clientes**: [Segmentação de Clientes]https://github.com/lazarocordeirosilva/Segmentacao_Clientes/blob/main/notebook/Segmenta%C3%A7%C3%A3o%20de%20Clientes.ipynb 

- Neste notebook foi aplicado o algoritmo KMeans à base de dados, com suas dimensões reduzidas, a fim de identificar similiaridades entre os respondentes do questionário, agrupando-os em clusters.  

## Requisitos
Neste projeto, foi utilizada a versão 3.11.4 do Python

A versão do pip utilizada é a 23.3.1

A versão do git utilizada é a 2.42.0

Demais requisitos se encontram no arquivo requirements.txt

## Replicação
> [!NOTE]
> Para utilizar este projeto, é necessário clonar o repositório

```
git clone https://github.com/lazarocordeirosilva/Segmentacao_Clientes.git
```
> [!NOTE]
> Após isso, você pode instalar os pacotes nas versões utilizadas
```
pip install -r requirements.txt
```

## Principais Conclusões e Resultados
O projeto revelou que um dos clusters identificados contém clientes com maior propensão a comprar a microvan. Esses clientes se destacam por uma menor preocupação financeira, preferência por veículos maiores, maior número de filhos e mais milhas percorridas anualmente. Em termos de renda e idade, eles ocupam uma posição intermediária em comparação aos demais clusters, que incluem indivíduos de maior renda e idade mais avançada.

Após aplicar filtros de idade e sexo, observou-se que homens com 40 anos ou mais são os principais candidatos à compra da microvan. A combinação dessas informações sugere que campanhas de marketing focadas nesses clientes específicos teriam maior eficácia, com a possibilidade de também alcançar homens do segundo cluster, caso os recursos permitam uma abordagem mais ampla.

## Estrutura do Projeto

```
├── LICENSE
├── README.md               <- README.md com principais informações do projeto.
│
├── arquivos                <- Arquivo .pkl para continuação da análise de segmentação.
│
├── data
│   ├── microvan.csv        <- Base de dados utilizada no projeto.
│   
├── notebook                <- Notebooks do projeto 
│   ├── PCA - Redução Dimensionalidade
│   ├── Segmentação de Clientes
│
├── requisitos              <- Todas as bibiliotecas utilizadas (em cada versão). Arquivo gerado com 'pip freeze > requirements.txt'

