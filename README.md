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
```sql
create database Trabalho;
-- criar tabela funcionarios]
create table Funcionarios1( 
id_funcionarios int primary key,
nome_funcionarios varchar (100),
sobrenome_funcionarios varchar (100),
salario_funcionarios decimal (10,2) 
);
```
```sql
alter table Funcionarios1 add dataNascimento date;
-- criar tabela departamento
create table departamentos1( 
id_departamentos int primary key,
nome_departamentos varchar (100)
);
```
```sql
alter table Funcionarios1 add IDDepartamentos int; 
-- criar tabela projetos
create table projetos1(
id_projetos int primary key,
nome_projeto varchar(100)
);
```
```sql
-- criar tabela alocações 
create table alocacoes1( 
id_alocacoes int primary key,
id_funcionario int,
id_projeto int 
);
```
```sql
alter table funcionarios1 rename column sobrenome to apelido;

-- criar tabela clientes
create table clientes1( 
id_clientes int primary key,
nome_cliente varchar(100) 
);
alter table projetos1 add IDCcliente int;
```
```sql
-- criar tabela endereços
create table enderecos1( 
id_enderecos int primary key,
rua_enderecos varchar (100),
cidade_enderecos varchar (100), 
cep_enderecos int (8) 
);
```
```sql
alter table funcionarios1 add column IDendereço varchar (100);
alter table clientes1 rename column nome_cliente to nome_empresa;
-- crie uma tabela chamada pedidos
create table pedidos(
id_pedidos int primary key,
data_pedido date
);
```
```sql
alter table pedidos add column IDCliente int;
-- crie uma tabela itens pedidos
create table itens_pedidos( 
id_pedidos int primary key,
id_pedido int,
id_produto int
);
```
```sql
-- crie uma tabela chamada produtos
 create table produtos( 
 id_produtos int primary key, 
 nome_produto varchar (100),
 quantidade_produto int,
 valor_produto decimal (10,2)
 );
 ```
 ```sql
 alter table produtos rename column nome_produto to descricao_produto;
 -- crie uma tabela chamada estoque 
 create table estoques(
 id_estoques int primary key,
 quantidade_estoque int
 );
 ```
  ```sql
 alter table estoques add column IDproduto int; 
-- crie uma tabela chamada vendas 
create table vendas1( 
id_vendas int primary key,
data_venda date
);
 ```
   ```sql
 alter table vendas1 add column IDCliente int;
   ```