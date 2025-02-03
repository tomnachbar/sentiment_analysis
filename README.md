# Identificação de Análise de Sentimentos dos Clientes através das avaliações realizadas no portal de compras da Fashion Nova

![Uma ilustração ou montagem mostrando gráficos, nuvem de palavras e ícones de sentimento (feliz, neutro, triste](https://github.com/user-attachments/assets/832858c1-b567-46bb-ade7-39828064c9c9)


## 1. Compreensão do Negócio

Neste projeto, analisamos dados da Fashion Nova, um e-commerce popular de moda feminina, para extrair insights valiosos sobre a percepção dos clientes;
Os dados analisados foram gerados através de avaliações deixadas pelos clientes do período de 2016 a Agosto de 2024. E com essas informações pretendemos retirar insights valiosos para resolução das questões de negócio solicitadas.

### Objetivo
O objetivo dessas análises foram resolver algumas questões de negócio que foram solicitadas conforme abaixo:

Quais mercados apresentam melhor e pior desempenho?
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


## 4. Relatório de Análise Exploratória (EDA)

Utilizando o df.describe()

Alguns dados importantes que já nota-se com a primeira análise exploratória indica:

+ Existem dados ausentes que necessitam de limpeza e tratamento;
+ A Coluna de países contam com um total de 181 países únicos, sendo que nas ocorrências o Estados Unidos (US) aparece em 121.912 vezes indicando possivelmente que a maioria dos clientes são do EUA;
+ Também verifica-se que houve 92.203 ocorrências com apenas 1 avaliação, que pode-se entender que a maioria dos usuários avaliou apenas uma vez;
+ Na coluna Rating, a nota 5 representa mais de 90 mil ocorrências o que transmite a ideia de que os clientes estão satifeitos em sua grande maioria.
+ Na coluna de Review Title (Título da avaliação), a palavra que mais aparece é Great, o que indica uma resposta padrão deixada pelos usuários e que pode ser melhor explorada.
+ E por fim a coluna Review Text (Texto da avaliação), 

![image](https://github.com/user-attachments/assets/c33c2963-a408-4827-8560-eadcb2b0af0e)


## 5. Principais Análises
#### + 90.782 avaliações com nota 5, sendo que 75% das avaliações são com nota superior a 4;

![image](https://github.com/user-attachments/assets/e2a11aff-9472-4a02-b915-b89262864210)

#### Média de Avaliações dos últimos 3 anos com notas superiores a 4, sendo um crescimento exponencial em 2021, com notas de avaliações médias saindo de 1.5 para 4.31;

![image](https://github.com/user-attachments/assets/950e763a-e795-4066-a81c-49923a9aa0bc)

#### Ao realizar a análise do sentimento das palavras deixadas nas avaliações mais de 54% das palavras utilizadas são positivas sendo Love e Great as palavras que mais se repetem, as palavras neutras representam 40% e as negativas apenas 5%, conforme distribuição a seguir:

![Captura de tela 2025-02-03 152028](https://github.com/user-attachments/assets/81d2ce18-4f56-4415-8367-babd27a68f0d)
![Captura de tela 2025-02-03 151950](https://github.com/user-attachments/assets/4af91bdf-1abf-40fe-a2e2-557d35203d1a)

#### No entanto, ao plotar a nuvem de palavras negativas, as palavras que mais aparecem são Service e Customer, o que pode indicar que o serviço de atendimento ao cliente esta necessitando de atenção, como sugestão a empresa poderia implantar um serviço de pós vendas, o que pode minimizar o número de avaliações ruins e sanar problemas antes de uma possível avaliação.

![Captura de tela 2025-02-03 152018](https://github.com/user-attachments/assets/507c2362-0dda-4a3c-845e-ecf34318115d)

![image](https://github.com/user-attachments/assets/6046df7c-a669-4c05-880a-228d1c14fdc1)

## 6.Referências

[Biblioteca NLTK](https://www.nltk.org/)

[Dados do Kaggle](https://www.kaggle.com/datasets/syedafroz6284/fashion-nova-reviews/data)


#### Para mais detalhes faça o download do material que preparei com as principais análises disponível no link abaixo:

📌 [Baixe aqui a apresentação completa com insights detalhados](https://drive.google.com/file/d/13UlKIxqK63rXBphJgKwmz0JIVJgJcWTz/view?usp=sharing)







