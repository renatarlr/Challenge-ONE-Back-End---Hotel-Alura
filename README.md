# Challenge-ONE-Back-End---Hotel-Alura
 Construir suas próprias aplicações utilizando Java do básico ao avançado e sua própria API REST utilizando Spring com suporte especializado via Discord.



<p align="center" >
     <img width="600" heigth="400" src="https://github.com/renatarlr/Challenge-ONE-Back-End---Hotel-Alura/assets/129464869/12f7768d-45e6-4bad-9e29-90cfc9c5e2a8">

</p>

## <img width="64" height="64" src="https://img.icons8.com/nolan/64/1A6DFF/C822FF/java-coffee-cup-logo.png" alt="java-coffee-cup-logo"/> Tecnologias Utilizadas:

- Java
- Eclipse
- MySql
- Biblioteca JCalendar
- Plugin WindowBuilder </br>

## <img width="64" height="64" src="https://img.icons8.com/color/48/java-coffee-cup-logo--v1.png" alt="java-coffee-cup-logo--v1"/>Requisitos para utilizar o aplicativo:

- Java
- MySQL Server (no **localhost:3306**)

## ⚙️ Configurando o MySQL:

- Criando o Banco de Dados (O nome deve ser **hotel_alura;**)
```sql
CREATE DATABASE hotel_alura;
```
- Acessando o Banco de Dados criado

```sql
USE hotel_alura;
```
- Criando a Tabela de Usuários

```sql
create table usuarios(
nome varchar (50),
senha varchar (50)
);
```
- Inserindo Seu Usuário na Aplicação à Sua Preferência
```sql
insert into usuarios (nome,senha) values('O SEU NOME','A SUA SENHA');
```
- Criando a Tabela de Reservas
```sql
create table reservas(
id int not null auto_increment,
data_entrada date not null,
data_saida date not null,
valor varchar(50),
forma_de_pagar varchar(50)not null,
primary key (id)
);
```
- Criando a Tabela de Hóspedes
```sql
create table hospedes(
id int not null auto_increment,
nome varchar(50) not null,
sobrenome varchar(50)not null,
data_nascimento date not null,
nacionalidade varchar (50) not null,
telefone varchar (50) not null,
id_reserva int not null,
primary key (id),
foreign key (id_reserva) references reservas(id)
);
```








https://github.com/renatarlr/Challenge-ONE-Back-End---Hotel-Alura/assets/129464869/b81d59c6-ca8b-4c9b-a36d-e945d7fff118


# FIM...





