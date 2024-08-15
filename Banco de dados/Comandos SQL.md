[[SQL]]
# Básico
## Criando a base de dados
```SQL
CREATE DATABASE DATABASE_NAME;
```
## Selecionando a base de dados
```SQL
USE DATABASE_NAME;
```
## Criando tabelas
```SQL
CREATE TABLE TABLE_NAME{
	column_1 DATA_TYPE,
	column_2 DATA_TYPE
};
```
## Alterando tabelas
### Adicionando coluna
```SQL
ALTER TABLE TABLE_NAME
ADD COLUMN column_name DATA_TYPE;
```
### Removendo coluna
```SQL
ALTER TABLE TABLE_NAME
DROP COLUMN column_name;
```
### Modificando coluna
```SQL
ALTER TABLE TABLE_NAME
MODIFY COLUMN column_name DATA_TYPE;
```
## Deletando tabelas
```SQL
DROP TABLE TABLE_NAME;
```
## Inserindo registro
```SQL
INSERT INTO TABLE_NAME (column_name,...)
VALUES (value_column_1,...);
```
## Consultando registros
```SQL
SELECT * FROM TABLE_NAME;
```
## Deletando registro
```SQL
DELETE FROM TABLE_NAME WHERE column = x;
```
