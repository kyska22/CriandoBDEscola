# CriandoBDEscola

DESARROLLO
Instrucciones del proyecto
De acordo com os comandos aprendidos, programe códigos SQL para criar um banco de dados chamado ESCOLA e deixe-o pronto para o uso. Depois, pesquise qual é o comando utilizado para inserir uma tabela no banco de dados e siga as instruções:

1. crie uma tabela chamada ALUNO;  
2. defina os atributos da tabela;
3. adicione a chave primária de nome ID (identificador);
4. adicione um atributo nome do tipo varchar;
5. adicione um atributo e-mail do tipo varchar;
6. adicione um atributo endereço do tipo varchar.


Aqui está um conjunto de comandos SQL para criar o banco de dados "ESCOLA", criar a tabela "ALUNO" e adicionar os atributos especificados:

sql
Copy code
-- Criar o banco de dados ESCOLA
CREATE DATABASE ESCOLA;

-- Usar o banco de dados ESCOLA
\c ESCOLA;

-- Criar a tabela ALUNO
CREATE TABLE ALUNO (
    ID SERIAL PRIMARY KEY,
    nome VARCHAR(100),
    email VARCHAR(100),
    endereco VARCHAR(255)
);
Explicação dos comandos:

CREATE DATABASE ESCOLA;: Este comando cria o banco de dados chamado "ESCOLA".

\c ESCOLA;: Este comando conecta ao banco de dados "ESCOLA" recém-criado.

CREATE TABLE ALUNO (...): Este comando cria a tabela "ALUNO" com os atributos especificados dentro dos parênteses.

ID SERIAL PRIMARY KEY: Este comando cria uma coluna chamada "ID" que é um tipo de dado serial, o que significa que é autoincrementável. Também define esta coluna como a chave primária da tabela.

nome VARCHAR(100), email VARCHAR(100), endereco VARCHAR(255): Estes comandos criam as colunas "nome", "email" e "endereco" com os tipos de dados varchar, que podem armazenar cadeias de caracteres de até 100 e 255 caracteres, respectivamente.
