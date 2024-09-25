# Banco1
--Exercicios 25/09
--Joaquim Barbosa Guedes

```sql
-- criar tabela clientes
create table Clientes1(
id_cliente int primary key,
nome_cliente varchar (100),
email_cliente varchar (100),
data_nascimento date,
telefone_cliente varchar (15)
);
```
```sql
-- criar tabela com restrição de unico
create table Produtos1( 
id_produto int primary key, 
nome_produto varchar (100),
preco_produto decimal (8,2)
);
```
```sql
-- definição de tabela com data e criação padrãoptimize
create table Faturas1(
id_fatura int primary key,
data_criacao date,
valor_fatura decimal ( 10,2) 
);
```