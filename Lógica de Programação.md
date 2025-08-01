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
- Operador "E": representado por (&&). É o operador lógico de inclusão.<br>
Esse operador só devolve "true" quando todos os booleanos envolvidos forem "true".
- Operador "OU": representado por (||). Operador lógico de "alternativa".<br>
Só devolve "false" quando todos seus booleanos são "false".<br>
Se pelo menos um for "true", então o retorno é "true". 
- **Exemplo de como usar o operador "E":**
```
INICIO
IMPRIMA true && true 
IMPRIMA true && false
IMPRIMA false && true
IMPRIMA true && false && true

FIM
```
*Obs: nesse quarto caso, o computador vai comparar 2 booleanos de cada vez. A primeira operação é true && false = false. A segunda operação é o resultado da primeira mais true, ou seja, false && true = false*<br>
&nbsp;&nbsp;&nbsp;&nbsp;**Resultado do exemplo acima:**
```
True
False
False

False && true
False
```
- **Exemplo de como usar o operador "OU":**
```
INICIO
IMPRIMA true || true 
IMPRIMA true || false
IMPRIMA false || true
IMPRIMA true || false || true

FIM
```
&nbsp;&nbsp;&nbsp;&nbsp;**Resultado do exemplo acima:**
```
True
True
True
True || true 
True
```
## Tabela Verdade
```
|     A     |     B    |  A && B  |   A || B  |
|-----------|----------|----------|-----------|
| ✅ true  | ✅ true  | ✅ true  | ✅ true  |
| ✅ true  | ❌ false | ❌ false | ✅ true  |
| ❌ false | ✅ true  | ❌ false | ✅ true  |
| ❌ false | ❌ false | ❌ false | ❌ false |
```

## Teste de Bullet Lista:<br>
A ordem da expressão lógica que os operadores serão resolvidos pelo computador e a ordem que devemos pensar
  - Prioridades:
    - Parênteses
    - Operadores Aritiméticos
    - Comparadores
    - Operadores Lógicos: "E" tem prioridade maior que "OU"
### Exercício 1
```
INICIO

IMPRIMA false || true || false

FIM
```
<details>
  <summary>Clique aqui para mostrar o resultado</summary>
 
Para resolver essa operação de dois em dois, separe por parênteses:<br>
**(False || true) || false**<br>

Agora resolva a questão entre parênteses:<br>
**True || false**<br>

Resultado:<br>
**True**
</details>

### Exercício 2
```
INICIO

IMPRIMA (false || true) && !true

FIM
```
<details>
  <summary>Clique aqui para mostrar o resultado</summary>
 
Primeiro resolva a questão entre parênteses:<br>
**True && !true**<br>
 
Agora resolva o operador (!):<br>
**True && false**<br>

Resultado final:<br>
**False**
</details>

### Exercício 3
```
INICIO
VARIAVEIS
  var1, var2, var3

var1 <- true
var2 <- false
var3 <- !var2

IMPRIMA (true && (!var1 || var2)) && !var3

FIM
```
<details>
  <summary>Clique aqui para mostrar o resultado</summary>

Conversão das variáveis no valor booleano:<br>

var1 <- true<br>
var2 <- false<br>
var3 <- true<br>
 
Primeiro resolva a questão entre parênteses interno:<br>
**(True && (!true || false)) && !true**<br>
**(True && (false || false)) && !true**<br>
**(True && false) && !true**<br>
 
Agora resolva a questão entre parênteses externo:<br>
**False && !true**<br>

Por último resolva o operador (!):<br>
**False && false**<br>

Resultado final:<br>
**False**
</details>

### Exercício 4
```
INICIO
VARIAVEIS
  var1, var2, var3

var1 <- true
var2 <- false
var3 <- !var2

IMPRIMA ((5 > 7) && (!var1 || var2)) && var3

FIM
```
<details>
  <summary>Clique aqui para mostrar o resultado</summary>

Conversão das variáveis no valor booleano:<br>

var1 <- true<br>
var2 <- false<br>
var3 <- true<br>
 
Primeiro reescreva a expressão lógica substituindo as variáveis:<br>
**((5 > 7) && (!true || false)) && true**<br>
 
Agora resolva a questão entre parênteses com comparador maior que:<br>
**((False) && (!true || false)) && true**<br>

Novamente resolva a questão entre parênteses interno que resta:<br>
**(False && (false || false)) && true**<br>
**(False && False) && true**<br>

Resolva a questão entre parênteses "externo":<br>
**False && true**<br>

Resultado final:<br>
**False**
</details>

## Operações com Strings e Arrays
- Concatenação: Operador de adição aplicado a Strings. Diferentes pedaços de texto se juntam.
```
INICIO
VARIAVEIS
  nomeDoUsuario, mensagem

nomeDoUsuario <- Escreva "Digite seu nome"

mensagem <- "Olá, " + momeDoUsuario + ", como você está?"

IMPRIMA mensagem

FIM
```
Você pode usar operações de adição para juntar pedaços de texto que estão em strings e pedaços de texto que estão armazenados em variáveis. 
- Acessando elemento de um Array: definir qual elemento se quer acessar e identificar ele pela sua posição na lista. É conhecido como **índice**.
  - Na programação geralmente utiliza-se a seguinte simbologia: nomeDoArray[indice]. *Obs: vale incluir que, na programação a contagem de números começa a partir do ZERO*<br>
  Exemplo: listaDeAlunos <- ["Alex", "Alice", "Bruna", "Caio"]<br>
  Alex = 0, Alice = 1, Bruna = 2, Caio = 3.
```
INICIO
VARIAVEIS
  listaDeAlunos

listaDeAlunos <- ["Alex", "Alice", "Bruna", "Caio", "Eduador", "Eloisa"]

Para imiprimir o primeiro elemento ("Alex"), segue o exemplo abaixo::

IMPRIMA listaDeAluno[0]

Para atribuir um novo valor a um determinado elemento, segue o exemplo abaixo:

listaDeAluno[4] <- "Davi"

FIM
```
- Abaixo vamos aprender como verifica a quantidade de elementos dentro do Array. Para isso, utiliza-se a palavra COMPRIMENTO seguido de "listaDeAlunos" entre parênteses.
```
INICIO
VARIAVEIS
  listaDeAlunos, quantidadeDeAlunos

listaDeAlunos <- ["Alex", "Alice", "Bruna", "Caio", "Eduador", "Eloisa"]

quantidadeDeAlunos <- COMPRIMENTO(listaDeAlunos)

FIM
```
- Comprimento vs. Indice:
  - Comprimento: conta a quantidade de itens
  - Índice: começa a ser contado a partir do zero, não do um. Por isso, sempre é menor que o comprimento.<br>
Para acessar o último elemento da lista faça da seguinte forma:
```
INICIO
VARIAVEIS
  listaDeAlunos, ultimoAlunos

listaDeAlunos <- ["Alex", "Alice", "Bruna", "Caio", "Eduador", "Eloisa"]

ultimoAluno <- listaDeAlunos[COMPRIMENTO(listaDeAlunos) - 1]

FIM
```
- Para alterar a quandidade de itens de uma lista utilize a fórmula:
  - Adição: ADICIONA(nomeDoArray, item)
  - Remoção: REMOVA(nomeDoArray, indiceDoElemento)
- **Exemplo de adição:**
```
INICIO
VARIAVEIS
  listaDeAlunos, ultimoAlunos

listaDeAlunos <- ["Alex", "Alice", "Bruna", "Caio", "Eduador", "Eloisa"]

ADICIONA(listaDeAlunos, Gabriela)

FIM
```
&nbsp;&nbsp;&nbsp;&nbsp;*Obs: a Gabriela será adicionada no final da lista*
- **Exemplo de remoção:**
```
INICIO
VARIAVEIS
  listaDeAlunos, ultimoAlunos

listaDeAlunos <- ["Alex", "Alice", "Bruna", "Caio", "Eduador", "Eloisa"]

REMOVA(listaDeAlunos, 4)

FIM
```
## Estrutura Condicionais
Será utilizado fluxograma que são representados por quadrado e losango. Cada passo será representado por quadrado e cada tomada de decisão será representado por losango. 
- Condicional Simples:  executa uma ação somente se uma condição for verdadeira.
  - Exemplo: Se nota ≥ 5, então Aprovado.
- Condicional Composta: executa uma ação se a condição for verdadeira, e outra se for falsa.
  - Exemplo: Se nota ≥ 5, então Aprovado; senão, Reprovado.
- Condicional Aninhada: uma condicional dentro de uma condicional; como um ninho mesmo! 
- Escolha Caso: permite executar diferentes blocos de código com base em vários valores possíveis de uma variável. É usada quando há múltiplas alternativas específicas a serem tratadas.
   Exemplo em pseudocódigo:
```
Escolha nota:
  Caso 10:
    Mostrar "Excelente!"
  Caso 7:
    Mostrar "Bom!"
  Caso 5:
    Mostrar "Na média."
  Outro:
    Mostrar "Precisa melhorar."
```
- **Exemplificação de fluxograma 1 - Condicional Simples e Composta :** <br>
[Clique aqui para visualizar o fluxograma](https://ibb.co/Gfx3KjDW)

```
INICIO
VARIAVEIS
  notaFinal

notaFinal <- ESCREVA "Qual foi a sua nota?"

SE notaFinal >= 5 ENTAO
  IMPRIMA "Foi aprovado, parabens!"
SENAO
  IMPRIMA "Reprovado!"
FIMSE

FIM
```
*Obs: o comando FIMSE é utilizado para determinar o fim do bloco "SE".*<br>
*Obs²: IDENTAÇÃO - Algumas linguagens não funcionam sem a identação adequada! É importante na organização do seu código.*
- **Exemplificação de fluxograma 2 - Condicional Aninhada** <br>
[Clique aqui para visualizar o fluxograma](https://ibb.co/GYq1zxh)
```
INICIO
VARIAVEIS
  notaFinal

notaFinal <- ESCREVA "Qual foi a sua nota?"

SE notaFinal >= 5 ENTAO
  IMPRIMA "Foi aprovado, parabens!"
SENAO
  SE novaFinal >= 3 ENTAO
    IMPRIMA "Você está de recuperação"
  SENAO
    IMPRIMA "Reprovado!"
  FIMSE
FIMSE

FIM
```
- **Exemplo de como usar o escolha caso** <br>
```
INICIO
VARIAVEIS
  notaFinal

notaFinal <- ESCREVA "Qual foi a sua nota?"

ESCOLHA notaFinal
  CASO 0
    IMPRIMA "Estou aqui caso precise de ajuda"
  CASO 5
    IMPRIMA "Essa foi por pouco"
  CASO 10
    IMPRIMA "Aluno exemplar!"
  OUTROCASO
    IMPRIMA "Nada a declarar"
FIMESCOLHA

FIM
```
