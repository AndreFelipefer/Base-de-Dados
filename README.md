# Base-de-Dados-Animais.
Este conjunto de exercícios utiliza um arquivo SQL chamado Tab_animais.sql para realizar diversas operações em uma base de dados de animais

1- Selecione todos os animais
```SQL
SELECT *
From TAB_ANIMAIS;
```
![image](https://github.com/AndreFelipefer/Base-de-Dados-Animais./assets/129207232/9d555ec0-70e3-4cc0-9d67-c0872e004928)

2- Selecione todos os animais que pesam menos que 13.1
```SQL
Select * from
TAB_ANIMAIS
Where peso and peso <14;
```
![image](https://github.com/AndreFelipefer/Base-de-Dados-Animais./assets/129207232/e3c751b2-bace-4dcd-9df3-bc3abcf92cc7)

3- Selecione todos nasceram entre fevereiro e dezembro de 2015
```SQL
SELECT *
FROM tab_animais
WHERE data_nascimento BETWEEN '2015-02-01' AND '2015-12-31';
```
![image](https://github.com/AndreFelipefer/Base-de-Dados-Animais./assets/129207232/a8459768-a6c2-4b73-85fd-633552ff86e6)


4- Selecione todos os animais brancos que pesam menos que 15.0
```sql
Select *
From TAB_ANIMAIS
Where cor ='branco' 
And peso > '15.0';
```
![image](https://github.com/AndreFelipefer/Base-de-Dados-Animais./assets/129207232/f72b57ae-760f-4231-9795-191515b20b4c)

5- Selecione nome, cor e peso de todos cujo nome comece com ’B’
```SQL
Select nome, cor, peso
From TAB_ANIMAIS
Where nome like 'B%';
```
![image](https://github.com/AndreFelipefer/Base-de-Dados-Animais./assets/129207232/5e0a3b2d-6f3b-43d1-be6e-5d71fb7f624b)

6- Selecione nome, cor e peso de todos com cor vermelha, amarela, marrom e laranja
```SQL
Select nome, cor, peso
From TAB_ANIMAIS
Where cor in ('vermelho','amarelo', 'marrom', 'laranja');
```
![image](https://github.com/AndreFelipefer/Base-de-Dados-Animais./assets/129207232/1001da74-8f13-4731-83f8-c79ae734a521)

7- Selecione nome, cor, data de nascimento e peso de todos ordenados pelos mais jovens
```SQL
Select nome, cor, data_nascimento , peso
From TAB_ANIMAIS
Order by data_nascimento;
```
![image](https://github.com/AndreFelipefer/Base-de-Dados-Animais./assets/129207232/cb866878-d887-470a-be40-a1793114ed7a)

8- Selecione todos os animais cujo nome comece com 'C' e não sejam brancos
```SQL
SELECT *
FROM tab_animais
WHERE nome LIKE 'C%' AND cor != 'Branco';
```
![image](https://github.com/AndreFelipefer/Base-de-Dados-Animais./assets/129207232/600d94be-4c96-4de7-9d45-e68371f6b6d1)

9- Selecione todos os animais cujo nome contenha 'ba'
```SQL
SELECT * 
From TAB_ANIMAIS 
Where nome 
Like 'Ba%';

```
![image](https://github.com/AndreFelipefer/Base-de-Dados-Animais./assets/129207232/690ef258-20e4-4685-9e16-67865620ba11)

10-Selecione todos os animais com peso entre 13.0 à 15.0,
```SQL
SELECT * 
From TAB_ANIMAIS 
Where peso 
BETWEEN 13.0 
And 15.0;
```
![image](https://github.com/AndreFelipefer/Base-de-Dados-Animais./assets/129207232/d99a3bfa-9700-4b14-af9a-122f664055bc)


11- Selecione todos os animais que o peso não seja maior que 30, com cor amarelo ou roxo e nascidos depois de 2012
```SQL
SELECT *
FROM TAB_ANIMAIS
WHERE peso <= 30.0
AND cor IN ('amarelo', 'roxo')
AND data_nascimento > '2012-01-01';
```
![image](https://github.com/AndreFelipefer/Base-de-Dados-Animais./assets/129207232/b4ea498a-5808-40f9-b5d2-a4eee546eebe)


12- (Desafio) Selecione todos os capricornianos
```SQL
SELECT *
FROM tab_animais
WHERE MONTH(data_nascimento) = 12 AND DAY(data_nascimento) >= 22 OR MONTH(data_nascimento) = 1 AND DAY(data_nascimento) <= 19;
```
![image](https://github.com/AndreFelipefer/Base-de-Dados-Animais./assets/129207232/5fca20bf-4611-4a20-a62b-49ca649e94dc)


12- (Desafio) Selecione todos os animais com nome formado por mais de uma palavra.
```SQL
SELECT *
FROM tab_Animais
WHERE INSTR(Nome, ' ') > 0;
```
![image](https://github.com/AndreFelipefer/Base-de-Dados-Animais./assets/129207232/ad81f2e6-71aa-4eda-a560-b2d04d0f8ec6)

# Modelos DER Tabelas Animais / Produtos / Filme: 
Tab_Animais - 

![Animal](https://github.com/AndreFelipefer/Base-de-Dados-Animais./assets/129207232/01410839-8827-487f-a62f-0651466cce2a)

Tab_Filme -

![Filme](https://github.com/AndreFelipefer/Base-de-Dados-Animais./assets/129207232/a1e8a52a-bb65-458f-9784-7f96a7f40491)

Tab_Produto - 

![Produto](https://github.com/AndreFelipefer/Base-de-Dados-Animais./assets/129207232/60d36d5a-ccca-4335-acfa-b0fa0c5e09a2)

## Obrigadooo!






