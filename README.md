# Análise de Cancelamento de Cartões de Crédito

Este projeto tem como objetivo analisar os dados de clientes de uma empresa de cartões de crédito para entender quais características aparecem com mais frequência entre os clientes que cancelaram o cartão.

Durante a análise, observei que clientes com menos produtos contratados, menos transações e mais contatos com a empresa apresentaram maior tendência ao cancelamento. Já o tipo de cartão não mostrou uma diferença relevante para explicar esse comportamento.

## Sobre o projeto

A análise foi realizada com uma base de dados que reúne informações de clientes ativos e de clientes que cancelaram o cartão. Após o tratamento dos dados, a base ficou com **10.126 clientes**, dos quais **16,1% cancelaram o cartão**.

## Objetivos

* Conhecer melhor os dados dos clientes.
* Comparar clientes ativos e clientes que cancelaram o cartão.
* Identificar padrões relacionados ao cancelamento.
* Entender quais informações podem ajudar a empresa a melhorar a retenção de clientes.

## Fonte dos dados

Base de dados pública disponível no Kaggle: [Credit Card Customers](https://www.kaggle.com/sakshigoyal7/credit-card-customers).

## Tecnologias utilizadas

* Python
* Pandas
* Plotly
* Google Colab

## Etapas da análise

1. Importação da base de dados em formato CSV.
2. Verificação e tratamento dos dados, incluindo a remoção da coluna de identificação e dos valores vazios.
3. Análise inicial das informações e da quantidade de clientes que cancelaram o cartão.
4. Comparação entre clientes ativos e cancelados por meio de tabelas e gráficos.
5. Interpretação dos resultados para identificar padrões relacionados ao cancelamento.

## Principais gráficos

Os gráficos abaixo ajudam a visualizar as diferenças entre clientes ativos e cancelados em alguns aspectos da base.

### Produtos contratados

[Ver gráfico de produtos contratados](produtos_contratados.png)

### Quantidade de transações

[Ver gráfico de quantidade de transações](qtde_transacoes.png)

### Valor das transações

[Ver gráfico de valor das transações](valor_transacoes.png)

### Contatos com a empresa

[Ver gráfico de contatos com a empresa](contatos.png)

## Principais conclusões

Durante a análise, identifiquei alguns padrões importantes:

* **Produtos contratados:** clientes com mais produtos contratados apresentaram menor tendência ao cancelamento.
* **Quantidade de transações:** clientes que realizaram mais transações apresentaram menor tendência ao cancelamento.
* **Valor das transações:** clientes com valores de transações mais altos também apresentaram menor tendência ao cancelamento.
* **Contatos com a empresa:** clientes que precisaram entrar em contato mais vezes apresentaram maior tendência ao cancelamento.

### Análise por tipo de cartão

O cartão Blue concentra a maior quantidade de cancelamentos, mas também representa a maior parte dos clientes da base. Sua taxa de cancelamento é de 16,1%, igual à taxa geral.

| Tipo de cartão | Clientes | Cancelados | Taxa de cancelamento |
| -------------- | -------: | ---------: | -------------------: |
| Blue           |    9.435 |      1.519 |                16,1% |
| Gold           |      116 |         21 |                18,1% |
| Silver         |      555 |         82 |                14,8% |
| Platinum       |       20 |          5 |                25,0% |

Apesar de o cartão Platinum apresentar a maior taxa de cancelamento, ele possui apenas 20 clientes na base. Por isso, essa diferença deve ser interpretada com cautela.

## O que aprendi com o projeto

Com este projeto, pratiquei o uso de Python e Pandas para importar, organizar e analisar dados. Também utilizei gráficos para comparar grupos de clientes e tabelas para facilitar a interpretação dos resultados.

A análise me ajudou a entender como os dados podem ser usados para identificar padrões e levantar questões importantes para uma empresa.

## Considerações finais

Os resultados indicam que a quantidade de produtos contratados, a movimentação dos clientes e a frequência de contatos com a empresa estão associados ao cancelamento de cartões nesta base de dados.

Essas informações podem servir como ponto de partida para investigar oportunidades de melhorar a experiência dos clientes e reduzir os cancelamentos. No entanto, a análise identifica associações entre os fatores observados e o cancelamento, mas não comprova que eles sejam suas causas diretas.


## Como acessar o projeto

O notebook completo está disponível neste repositório, no arquivo `.ipynb`. Ele foi desenvolvido no Google Colab e pode ser aberto na plataforma para consultar o código, as tabelas e os resultados da análise.
