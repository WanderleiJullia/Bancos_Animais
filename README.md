# Bancos_Animais
## Atividade a seguir possui o objetivo de inserir as seguintes informações dos animais; 

## 1º Selecione todos os animais;
![image](https://github.com/WanderleiJullia/Bancos_Animais/assets/144744092/d275361a-0928-497d-8098-0a4ebd668bcf)

## 2º Selecione todos os animais que pesam menos que 13.1;
![image](https://github.com/WanderleiJullia/Bancos_Animais/assets/144744092/8305001d-b2b5-4066-9000-23a39cd25d99)

## 3º Selecione todos nasceram entre fevereiro e dezembro de 2015; 
![image](https://github.com/WanderleiJullia/Bancos_Animais/assets/144744092/35fc3f79-6c3b-4e13-91c6-dec5bffd9265)

## 4º Selecione todos os animais brancos que pesam menos que 15.0;
![image](https://github.com/WanderleiJullia/Bancos_Animais/assets/144744092/6c92dd9d-efce-4c24-b3c3-158c85a0ecb9)

## 5º Selecione nome, cor e peso de todos cujo nome comece com ’B’;
![image](https://github.com/WanderleiJullia/Bancos_Animais/assets/144744092/e24fec26-f330-4090-bf25-a2fa7ccf0b63)

## 6º Selecione nome, cor e peso de todos com cor vermelha, amarela, marrom e laranja;
![image](https://github.com/WanderleiJullia/Bancos_Animais/assets/144744092/365d266b-e418-4d8a-81bb-cd6645110648)

## 7º Selecione nome, cor, data de nascimento e peso de todos ordenados pelos mais jovens;
![image](https://github.com/WanderleiJullia/Bancos_Animais/assets/144744092/afd72c01-70d7-4fa7-90fa-51be07e02291)

## 8º Selecione todos os animais cujo nome comece com 'C' e não sejam brancos;
![image](https://github.com/WanderleiJullia/Bancos_Animais/assets/144744092/5cb18271-2996-4ddb-8a0f-a2fa78a7233e)

## 9º Selecione todos os animais cujo nome contenha 'ba';
![image](https://github.com/WanderleiJullia/Bancos_Animais/assets/144744092/1bf142d2-5fc0-4efa-8829-19cb6f3064ac)

## 10º Selecione todos os animais com peso entre 13.0 à 15.0;
![image](https://github.com/WanderleiJullia/Bancos_Animais/assets/144744092/bce7e2f6-ece4-41cb-a954-3404b446c411)

## 11º Selecione todos os animais que o peso não seja maior que 30, com cor amarelo ou roxo e nascidos depois de 2012;
![image](https://github.com/WanderleiJullia/Bancos_Animais/assets/144744092/5c6af3aa-2854-4147-8321-cf5bb682afcb)

## 12º Crie um banco de dados para armazenar dados de Animais e Espécies. Um animal tem seu nome, data_nasc e peso. Uma espécie tem um nome e uma descrição.
![image](https://github.com/WanderleiJullia/Bancos_Animais/assets/144744092/cb3ef98d-c610-4368-95d0-54e465506c6d)

```SQL
create table animal(
Nome varchar(50),
data_nasc date, 
peso decimal(10,02)
);

insert into animal (Nome, data_nasc, peso) values ('Bailey', '2023-01-23', 10.2);
insert into animal (Nome, data_nasc, peso) values ('Lili', '2022-02-25', 09.2);
insert into animal (Nome, data_nasc, peso) values ('Bumba', '2021-01-24', 11.02);
insert into animal (Nome, data_nasc, peso) values ('Milk ', '2022-09-05', 25.09);
insert into animal (Nome, data_nasc, peso) values ('Leão', '2015-03-12', 18.5);
insert into animal (Nome, data_nasc, peso) values ('Elefante', '2010-07-25', 45.75);
insert into animal (Nome, data_nasc, peso) values ('Girafa', '2018-11-02', 12.25);
insert into animal (Nome, data_nasc, peso) values ('Escobar', '2021-06-09', 10.2);

 create table especie(
 Nome varchar(90),
 Descricao text
 ); 
 
insert into especie (Nome, Descricao) values ('Biver', 'Cachorro de porte pequeno');
insert into especie (Nome, Descricao) values ('gato', 'Femea, calma');
insert into especie (Nome, Descricao) values ('Vira lata', 'Cachorro de porte medio achado em rua');
insert into especie (Nome, Descricao) values ('Macaco', 'De uma especie calma, para educar em casa');
insert into especie (Nome, Descricao) values ('Gato', 'Nome dato por sua cor laranja');
insert into especie (Nome, Descricao) values ('Cachorro', 'De grande porte');
insert into especie (Nome, Descricao) values ('Cachorro', 'Cachorro de porte grande e alto');
insert into especie (Nome, Descricao) values ('Cobra', 'CObra domesticada');
 ``` 

## 13º Crie um banco de dados para registrar dados de Produtos e Marcas. Um produto deve ter nome, preço de custo, preço de venda, data de validade e marca. Uma marca deve ter, nome, site oficial e telefone.
![image](https://github.com/WanderleiJullia/Bancos_Animais/assets/144744092/771d7a33-c258-4a36-92d6-523121b8fd8a)

``` SQL 
CREATE TABLE Produtos (
    id INT AUTO_INCREMENT PRIMARY KEY,
    nome VARCHAR(255) NOT NULL,
    preco_custo DECIMAL(10, 2) NOT NULL,
    preco_venda DECIMAL(10, 2) NOT NULL,
    data_validade DATE NOT NULL,
    marca VARCHAR(255) NOT NULL
);

INSERT INTO Produtos (nome, preco_custo, preco_venda, data_validade, marca) VALUES
    ('Camiseta', 15.99, 29.99, '2023-12-31', 'Nike'),
    ('Notebook', 600.00, 999.99, '2024-06-30', 'Dell'),
    ('Celular', 200.00, 399.99, '2024-04-15', 'Samsung'),
    ('Tênis', 40.00, 79.99, '2023-12-31', 'Adidas'),
    ('Máquina de Café', 30.00, 59.99, '2024-02-28', 'Breville'),
    ('Tablet', 120.00, 249.99, '2024-03-15', 'Apple'),
    ('Fone de Ouvido', 10.00, 29.99, '2024-01-31', 'Sony'),
    ('Relógio', 50.00, 99.99, '2023-12-31', 'Casio');


CREATE TABLE Marcas (
    id INT AUTO_INCREMENT PRIMARY KEY,
    nome VARCHAR(255) NOT NULL,
    site_oficial VARCHAR(255),
    telefone VARCHAR(20)
);

INSERT INTO Marcas (nome, site_oficial, telefone) VALUES
    ('Nike', 'https://www.nike.com', '+1 (800) 344-6453'),
    ('Dell', 'https://www.dell.com', '+1 (800) 624-9897'),
    ('Samsung', 'https://www.samsung.com', '+1 (800) 726-7864'),
    ('Adidas', 'https://www.adidas.com', '+1 (800) 982-9337'),
    ('Breville', 'https://www.breville.com', '+1 (866) 273-8455'),
    ('Apple', 'https://www.apple.com', '+1 (800) 692-7753'),
    ('Sony', 'https://www.sony.com', '+1 (239) 245-6361'),
    ('Casio', 'https://www.casio.com', '+1 (800) 435-7732');
```

## 14º Crie um banco de dados para registrar dados de Filmes e Categorias. Um filme tem seu título, sinopse, estudio e categoria. Uma categoria deve ter nome e público alvo.
![image](https://github.com/WanderleiJullia/Bancos_Animais/assets/144744092/d5109a61-121b-4967-b6a0-301b4271a2e3)

``` SQL
CREATE TABLE Filmes (
    id INT AUTO_INCREMENT PRIMARY KEY,
    titulo VARCHAR(255) NOT NULL,
    sinopse TEXT,
    estudio VARCHAR(255),
    categoria VARCHAR(50)
);

INSERT INTO Filmes (titulo, sinopse, estudio, categoria) VALUES
    ('Matrix', 'Um hacker descobre uma realidade virtual dominada por máquinas.', 'Warner Bros.', 'Ficção Científica'),
    ('O Senhor dos Anéis', 'Uma jornada épica em um mundo de fantasia.', 'New Line Cinema', 'Fantasia'),
    ('Titanic', 'Um romance a bordo do famoso navio que naufragou.', '20th Century Fox', 'Romance'),
    ('Jurassic Park', 'Dinossauros são trazidos de volta à vida em um parque temático.', 'Universal Pictures', 'Aventura'),
    ('Pulp Fiction', 'Histórias entrelaçadas de crime e redenção.', 'Miramax Films', 'Crime'),
    ('Forrest Gump', 'A vida de um homem comum que presencia eventos históricos.', 'Paramount Pictures', 'Drama'),
    ('Star Wars', 'A saga de uma galáxia muito, muito distante.', 'Lucasfilm', 'Ação'),
    ('E.T. - O Extraterrestre', 'Um garoto faz amizade com um alienígena perdido na Terra.', 'Universal Pictures', 'Família');


CREATE TABLE Categorias (
    id INT AUTO_INCREMENT PRIMARY KEY,
    nome VARCHAR(255) NOT NULL,
    publico_alvo VARCHAR(255)
);

INSERT INTO Categorias (nome, publico_alvo) VALUES
    ('Ação', 'Adultos'),
    ('Comédia', 'Todas as idades'),
    ('Drama', 'Adultos'),
    ('Ficção Científica', 'Jovens e adultos'),
    ('Animação', 'Crianças'),
    ('Terror', 'Adultos'),
    ('Romance', 'Jovens e adultos'),
    ('Documentário', 'Todas as idades');
```










