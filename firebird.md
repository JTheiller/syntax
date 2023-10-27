A linguagem SQL (Structured Query Language) é uma ferramenta fundamental no mundo da gestão de bancos de dados, e compreender a sua sintaxe é essencial para extrair informações e manipular dados de forma eficaz. Neste documento, exploraremos a sintaxe da linguagem, desvendando os principais componentes que a compõem. Vamos mergulhar nos conceitos essenciais, desde a criação de tabelas e consultas simples até operações avançadas de junção, agregação e subconsultas. Ao final desta exploração, você terá uma compreensão sólida da estrutura e gramática da linguagem SQL, permitindo que você aproveite ao máximo seu potencial no gerenciamento e análise de dados. Vamos começar essa jornada pelo fascinante mundo da sintaxe SQL.

## Operadores
### Aritméticos - Arithmetic operators
- `+` Somar
- `-` Subtrair
- `*` Multiplicar
- `/` Dividir
### Operadores de comparação - Comparison operator
- `=` igual
- `<>` diferente
- `>` Maior que
- `>=` Maror ou igual
- `<` Menor que
- `<=` Menor ou igual
- `is null` é nulo
- `is not null` não é nulo
### Operadores de funções - Function operator
- `start with` Iniciado com
- `container` Contenha
- `like [value]%` Inicie com
- `like %[value]` Termine com
- `like %[value]%` Contenha 
- ### Operadores lógicos - Comparison operator
- `AND` E
- `OR` OU
- `NOT` NÂO

## Select - Selecionar dados
### Todos os campos - All fields
```sql
select * from PRODUTOS
```
|ID|DESCRICAO|PRECO|CUSTO|ESTOQUE|
|-|-|-|-|-|
|1|PRODUTO TESTE|10|5|2|
### Campos especificos - Specific fields
```sql
select ID, DESCRICAO from PRODUTOS
```
|ID|DESCRICAO|
|-|-|
|1|PRODUTO TESTE|

### Contatenar - Concatenation operator
- `||` Duplo pipe
```sql
select ID || ' - ' || DESCRICAO as CAMPO_UNICO from PRODUTOS
```
|CAMPO_UNICO|
|-|
|1 - PRODUTO TESTE|
### Parametros input - Input parameters
- `:[name]` Simbolo "Dois pontos" seguido do nome do parametro

## Where - Filtro
- Listar todos os campos da tabela PRODUTOS
- Definindo o seguinte filtro de dados
- ID `menor ou igual a 1000`
- e (DESCRICAO `inicie com A` ou DESCRICAO `começe com B`)
```sql
select * from PRODUTOS
where
ID <= 1000
and ( (DESCRICAO like 'A%') or (DESCRICAO start with 'B%') )
```

## First - Primeiros X registros
```sql
select first 10
ID, DESCRICAO
from PRODUTOS
```

## Skip - Pular X registros
```sql
select skip 10
ID, DESCRICAO
from PRODUTOS
```
```sql
select first 10 skip 20
ID, DESCRICAO
from PRODUTOS
```

## Rows - Faixa de registros
```sql
select
ID, DESCRICAO
from PRODUTOS
rows 1 to 10;
```

## ALIAS - Apelido de campos tabelas ou sql
```sql
select
P.ID
from PRODUTOS AS P
```
```sql
select
P.ID
from PRODUTOS P
```
```sql
select
ID AS CODIGO
from PRODUTOS
```
## Join - Relacionamentos
```sql
select
  PRODUTOS.ID,
  PRODUTOS.DESCRICAO,
  PRODUTOS.MARCA_ID,
  MARCAS.DESCRICAO AS DESCRICAO_MARCA
from
  PRODUTOS
join MARCAS on MARCAS.ID = PRODUTOS.MARCA_ID
```
|ID|DESCRICAO|MARCA_ID|DESCRICAO_MARCA|
|-|-|-|-|
|1|PRODUTO TESTE|1|NIKE|

## COALESCE - Se estiver nulo, considerar valor informado
```sql
select
ID,
COALESCE(CUSTO, 0)
from PRODUTOS
```
|ID|CUSTO|
|-|-|
|1|NULL|

|ID|CUSTO|
|-|-|
|1|0|
