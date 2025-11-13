# Estudo 001 de Power BI

Esse projeto foi feito em referência ao curso 'Excel + Power BI + DAX — 7 Cursos em 1 Formação Especialista' do Jilson Santana na Udemy no link: https://www.udemy.com/course/curso-de-excel-avancado-2016-para-se-tornar-especialista/

## Dados

Os dados que compões os dashboards são oriundos do próprio curso, são dados de uma rede de hotel fictícia onde existe uma rede de clientes, que são empresas de viagem, e fazem a venda de pacotes pra essa rede de hotel chamada ‘Hotéis Smart’.

Dessa forma foi necessário criar um modelo de dados dentro do Power BI, o modelo é composto de 5 tabelas, sendo elas:

- **Cliente:** São informações sobre as agências de viagens;
- **Funcionários:** São os funcionários dos clientes que fizeram alguma reserva nos hotéis;
- **Hotéis Smart:** São as informações dos Hotéis;
- **ReservasDatas:** É uma tabela criada pra guardar a data da reserva. 
- **Medidas:** Tabela criada pra guardas as medidas que foram usadas no dashboard ou não, aqui existem algumas medidas que não foram incluídas no dashboard a caráter somente de estudo.
- **Reservas:** Tabela principal que aglomera as informações da reserva que foi realizada em determinado hotel.

Os dados de cada tabela vêm de arquivos CSV com o mesmo nome da tabela, fizemos a carga desses arquivos pro Power BI e em seguida criamos as tabelas citadas a cima.

As únicas exceções são para as tabelas de datas de reservas e de medidas.

Todas as medidas foram criadas usando as funções DAX.

#### Modelo de Dados:

<img src="https://github.com/ciceroalcantara/analises/blob/main/dashboards/001_hoteis_smart/modelo_de_dados.png"/>

## Visões

No **primeiro** dashboard temos visão para algumas métricas, entre elas estão:
- **Taxa de conversão:** É uma medida que diz o número de reservas que foram finalizadas dividido pelo número total de reservas.
- **Receita por tipo de passageiro:** É uma medida que diz a porcentagem que o tipo de passageiro representa do todo.
- **Receita:** É a medida que diz a receita total que os hotéis tiveram, a receita pode variar de acordo com o dado que o cliente está analisando.
- **Margem de lucro:** É a medida que divide o lucro total pela receita total.
- **Receita por forma de pagamento:** É um gráfico que diz quantos porcento uma determinada forma de pagamento representa na receita total.
- **Canais de venda:** É um gráfico que mostra a porcentagem que representa os canais de vendas das reservas.
- **Receita por funcionários:** É um gráfico que mostra quanto representa o funcionário no total de receita, assim a gente fica sabendo qual funcionário performou melhor nas vendas.

#### Dashboard 1:

<img src="https://github.com/ciceroalcantara/analises/blob/main/dashboards/001_hoteis_smart/dashboard_01.png"/>

No **segundo** dashboard temos a visão do local em que as reservas foram feitas:
- **Número de reservas por país:** É um gráfico do tipo mapa que mostra através de bolhas a quantidade de reservas que foram feitas por clientes do país.
- **Receita total por país:** É um gráfico que mostra o total de receita dividida por país.
- **Top 10 clientes:** Uma tabela que mostra os clientes que mais performaram, pode ser filtrado por país.

#### Dashboard 2:

<img src="https://github.com/ciceroalcantara/analises/blob/main/dashboards/001_hoteis_smart/dashboard_02.png"/>

No **terceiro** dashboard é uma tabela de detalhe que fica oculta, o cliente só terá acesso caso filtre um hotel em especifico do dashboard 1 usando 'Drill-through'.

O gráfico mostra especialmente a porcentagem de crescimento de um determinado hotel ao longo do ano, comparado com o ano anterior.

#### Dashboard 3:

<img src="https://github.com/ciceroalcantara/analises/blob/main/dashboards/001_hoteis_smart/dashboard_03.png"/>
