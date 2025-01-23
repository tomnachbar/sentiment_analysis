# Identificação de Análise de Sentimentos dos Clientes através das avaliações realizadas no portal de compras da Fashion Nova


## 1. Compreensão do Negócio

Nesse projeto iremos visualizar e entender algumas análises realizadas acerca de um conjunto de dados da Fashion Nova, um popular site de roupas feminina;
Os dados analisados foram gerados através de avaliações deixadas pelos clientes do período de 2016 a Agosto de 2024. E com essas informações pretendemos retirar insights valiosos para resolução das questões de negócio solicitadas.

### Objetivo
O objetivo dessas análises foram resolver algumas questões de negócio que foram solicitadas conforme abaixo:

Estamos performando bem em todos os mercados?
Como está a satisfação dos nossos clientes?
Estamos melhores no período atual comparado com o passado?
Existe diferença entre a percepção da marca para clientes engajados ou não engajados?

## 2. Entendendo os Dados Disponíveis

O conjunto de dados contém avaliações de clientes, de compras realizadas entre o ano de 2016 a agosto de 2024. 
A divisão de colunas foi realizada em Nome do Cliente, Link, País, Contagem de Avaliações, Datas, e a Avaliação. Após a limpeza iremos trabalhar com um conjunto com 131.802 ocorrências.
### Resumo das colunas:
  + Reviewer Name: Nome do cliente que está avaliando o pedido
  + Profile Link: Link do Perfil do Cliente
  + Profile IDs: Essa coluna foi criada para atribuir um código único a cada avaliador, já que para realizar as análises foram encontrados nomes iguais ou repetidos, o que comprometeria a efetividade dos resultados.
  + Country: Código dos países de maneira resumida
  + Country Name: Coluna criada com nomes por extenso para melhor compreensão e facilidade de leitura
  + Review Count: Número de contagem de avaliações
  + Review Date: Data da Avaliação
  + Rating: Nota da Avaliação
  + Review Title: Título da Avaliação
  + Review Text: Texto escrito na Avaliação
  + Date of Experience: Data de Experiência ou do Pedido
      

## 3. Preparação dos Dados

+ Fora realizado a inclusão de uma nova coluna com ID’s únicos de avaliadores, pois foram encontrados nomes duplicados nos dados disponíveis. 
+ As linhas com espaços vazios foram eliminadas a fim de não prejudicar o resultado final das avaliações.
+ Também fora adicionada uma nova coluna de país com os nomes por extenso para melhor entendimento dos dados.

## 4. Principais Insights

+ 90.782 avaliações com nota 5.
+ 75% das avaliações com nota superior a 4.
+ Crescimento exponencial em 2021, com notas de avaliações médias saindo de 1.5 para 4.31

## 5. Relatório de Análise Exploratória (EDA)


