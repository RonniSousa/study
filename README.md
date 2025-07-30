# Lógica De Programação 
- Lógica e algoritmos
  * Lógica: é a ciência do pensamento, a forma das pessoas pensarem. É estudada tanto na matemática quanto na filosofia.
  * Algoritmo: é uma sequência de instruções para solucionar um problema.
 - Linguagem de programação: quanto mais próxima da binária, pode-se dizer que é uma linguágem de baixo nível. Quanto mais próximo da linguagem natural/humana, diz-se alto nível. 

## Variáveis
- O que são variáveis? 
São como depósitos como caixas e gavetas, na qual são nomeadas para guardar "coisas".
- Criação de variáveis
  * Declaração: etapa que se cria e se dá nome à variável. Ela fica armazenada na memória do computador.
  * Atribuição: etapa que se armazena informação dentro da variável.
- **Exemplo:**
```
INICIO
VARIAVEIS
  nomeDoUsuario
nomeDoUsuario <-ESCREVA "Digite seu nome"

IMPRIMA nomeDoUsuario

FIM
```
- Na programação é comum ver o sinal de = (igual) para a atribuição de variáveis.
### Tipos De Variável 
- String / Texto: representado entre aspas "".
- Number: representado por número.
- Array / lista: pode armazenar mais de um item. São representados por [ ] (colchetes) para representar uma lista. Exemplo: ["item 1", "item 2"].
- Boolean: é a variável denominada de verdadeira ou falsa / true or false.
- **Exemplo:**
```
INICIO
VARIAVEIS
 nome, idade, profissao, entrouNoBarril
nome <- "Chaves"
idade <- 18
profissao <- ["Sem teto", 18, "Mendigo"]
entrouNoBarril <- true

FIM
```
Obs: as variáveis podem ser misturadas dentro do array/lista. Pode ser misturada com textos e números ou até mesmo criar uma lista dentro de uma lista. 
## Operadores Aritméticos e Comparadores
 - Variáveis Number
    - Operadores aritméticos: soma (+), subtração (-), multiplicação (*) e divisão (/).
    - Resto da divisão: representado por (%). Há casos em que dividir um número pelo outro não da o resultado redondo, por exemplo: 20 dividido por 3 resulta em 6 com sobra igual a 2, essa sobra é o resto da divisão. Esse operador é utilizado para verificar a paridade de um número, ou seja, para ver se o número é par ou ímpar.
 - Comparadores: são operadores que permitem comparar dois valores. O resultado sempre será um valor booleano (True or False).
    - Igualdade: representado por (===). Esse operador verifica se tanto o valor quanto o tipo de variáveis são iguais e também pode ser utilizado para comparar o tipo texto.<br>
    Se sim, True<br>
    Se não, False
    - Desigualdade: representado por (!==). Esse operador verifica se tanto o valor quanto o tipo de variáveis são desiguais.<br>
    Se sim, True<br>
    Se não, False<br>
    *Obs: na programação o exclamação (!) significa **NÃO**.*
    - Maior que: representado por (>). Só funciona com números.<br>
    **True** se o primeiro número for maior que o segundo.<br>
    **False** se o primeiro número não for maior que o segundo.
    - Menor que: representado por (<) Só funciona com números.<br>
    **True** se o primeiro número for menor que o segundo.<br>
    **False** se o primeiro número não for menor que o segundo.
- **Exemplo de como usar soma e subtração:**
```
INICIO
VARIAVEIS
 precoDoMelao, precoDaUva, total
precoDoMelao <- 4
precoDaUva <- 2

total <- precoDoMelao + precoDaUva

FIM
```
- **Exemplo de como calcular o troco da operação:**
```
INICIO
VARIAVEIS
 precoDoMelao, precoDaUva, total, pagamentoEmDinheiro, troco
precoDoMelao <- 4
precoDaUva <- 2

total <- precoDoMelao + precoDaUva

pagamentoEmDinheiro <- 20

troco <- pagamentoEmDinheiro - total

FIM
```
- **Exemplo de como usar multiplicação e divisão:**
```
INICIO
VARIAVEIS
  caixasDeBombom, bombomPorCaixa, pessoas, totalDeBombons, bombonsPorPessoa

caixasDeBombom <- 5
bombonsPorCaixa <- 12
pessoa <- 6

totalDeBombons <- caixasDeBombom * bombonsPorCaixa
bombonsPorPessoa <- totalDeBombons / pessoas

FIM
```
- **Exemplo de como usar o resto da divisão:**
```
INICIO
VARIAVEIS
  dividando, divisor, resto

dividendo <- 20
divisor <- 3
resto <- 20 % 3

FIM
```
- **Exemplo de como usar o comparador de igualdade:**
```
INICIO
IMPRIMA 1 === 1
IMPRIMA 1 === 2
IMPRIMA "João" === "Maria"
IMPRIMA "1" === 1

FIM
```
&nbsp;&nbsp;&nbsp;&nbsp;**Resultado do exemplo acima:**
```
True
False
False
False
```
- **Exemplo de como usar o comparador de desigualdade:**
```
INICIO
IMPRIMA 1 !== 1
IMPRIMA 1 !== 2
IMPRIMA "João" !== "Maria"
IMPRIMA "1" !== 1

FIM
```
&nbsp;&nbsp;&nbsp;&nbsp;**Resultado do exemplo acima:**
```
False
True
True
True
```
- **Exemplo de como usar o comparador maior que:**
```
INICIO
IMPRIMA 1 > 2
IMPRIMA 2 > 1
IMPRIMA 1 > 1
IMPRIMA 1 >= 1
IMPRIMA 1 > 2 > 3

FIM
```
&nbsp;&nbsp;&nbsp;&nbsp;**Resultado do exemplo acima:**
```
False
True
False
True
ERROR: o computador não consegue fazer mais de uma comparação de uma só vez.
```
- **Exemplo de como usar o comparador menor que:**
```
INICIO
IMPRIMA 1 < 2
IMPRIMA 2 < 1
IMPRIMA 1 < 1
IMPRIMA 1 <= 1

FIM
```
&nbsp;&nbsp;&nbsp;&nbsp;**Resultado do exemplo acima:**
```
True
False
False
True
```
## Operadores Lógicos
- Operador "E": representado por (&&). É o operador lógico de inclusão. Esse operador só devolve "true" quando todos os booleanos envolvidos forem "true".
- **Exemplo de como usar o operador "E":**
```
INICIO
IMPRIMA true && true 
IMPRIMA true && false
IMPRIMA false && true
IMPRIMA true && false && true

FIM
```
&nbsp;&nbsp;&nbsp;&nbsp;*Obs: nesse quarto caso, o computador vai comparar 2 booleanos de cada vez. A primeira operação é true && false = false. A segunda operação é o resultado da primeira mais true, ou seja, false && true = false*<br>
&nbsp;&nbsp;&nbsp;&nbsp;**Resultado do exemplo acima:**
```
True
False
False

False && true
False
```
