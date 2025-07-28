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
 * Operadores aritméticos: soma (+), subtração (-), multiplicação (*) e divisão (/).
- **Exemplo:**
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
