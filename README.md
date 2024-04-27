# Processando e Transformando Dados com Power BI

## Passo 01 – Criação da instância Azure DB

1-Primeiro eu fiz a criação de uma instância na Azure para MySQL, logo depois fiz integração do Power BI com MySQL no Azure..

<img src="azure-captura.PNG">

## Passo 02 – Trasnformação de dados os Dados

Exclusão de todas as colunas my_row_id

Mudando o valor de Super_Ssn de NULL para 0 na tabela employee.

Mudando o tipo de dados da coluna Salary para decimal fixo em employee.

Mudando o tipo de dados da coluna Dno para texto em project.

Mudando o tipo de dados da coluna Pnumber e Dnum para texto em project.

Mudando o tipo de dados da coluna Dnumber para texto em departament.

Mudando o tipo de dados da coluna Dnumber para texto em deppt_locations.

Mudando o tipo de dados da coluna Pno para texto em works_on.

O employee com Super_Ssn com valor 0 é o gerente.

Todos os departamentos possuem um gerente associado.

Depois eu fiz o mesclar consultas employee e departament para criar uma tabela employee com o nome dos departamentos associados aos colaboradores. A mescla terá como base a tabela employee.



## Obs:

Tive que criar as tabeles sem constraint e relacionamentos, pois quando eu colocava igual estava no repositório no git hub, no Power Bi algumas tabelas ficavam vazias.

