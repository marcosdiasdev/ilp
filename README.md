# Apostila de Lógica de Programação

A **Lógica de Programação** é a técnica de encadear pensamentos para atingir determinado objetivo por meio de um computador ou outro sistema programável.

## Algoritmo

Podemos definir algoritmo como uma sequência finita e ordenada de passos para a resolução de um problema específico.

Para exemplificar, vamos começar com um algoritmo descritivo para um problema clássico do cotidiano: como fritar ovos?

```
-- Algoritmo para fritar ovos

1.	pegar frigideira, ovo, óleo e sal
2.	colocar óleo na frigideira
3.	acender o fogo
4.	levar a frigideira ao fogo
5.	esperar o óleo esquentar
6.	colocar o ovo
7.	colocar sal no ovo
8.	retirar quando pronto
```

Percebe que o algoritmo acima é basicamente uma receita? Algoritmos são exatamente como receitas.

## Programa de Computador

Um Programa de Computador é um algoritmo escrito com o uso de uma linguagem de computador, ou linguagem de programação, como C, Pascal, Java, JavaScript, PHP etc.

## Variável

Uma variável é um local na memória, um endereço que armazena um conteúdo.
Variáveis podem possuir nomes, seja `y` ou `x` ou qualquer outro nome.

### Nomenclatura de variáveis

Há algumas regras a serem seguidas ao nomear variáveis. Algumas linguanges de programação poderão apresentar padrões diferentes, mas há algumas convenções que devem ser sempre seguidas para manter o código legível e livre de erros:

- O nome de uma variável não deve conter espaços ou acentos
- O nome de uma variável não deve conter operadores
- O nome de uma variável não deve ser só um número
- Algumas linguagens de programação diferenciam letras maiúsculas de letras minúsculas, logo: `Nome` pode ser diferente de `nome`.


## Atribuição de valores

Atribuir um valor a uma variável é dar um valor a uma variável. É o mesmo que guardar um valor em um espaço da memória.

```
a = 4			
```
Pode ser lido como: variável a recebe 4.

```
nome = “José”
```
Pode ser lido como: variável nome recebe José.

Observe que o símbolo de igualdade, `=`, aqui é utilizado como operador de atribuição. Para igualdade, utilize `==`.

## Tipos de variáveis

O tipo de uma variável define o tipo de valor que ela poderá armazenar. Por exemplo, se precisamos armazenar um número inteiro, podemos criar uma variável do tipo **inteiro**; para armazenar nomes, utilizamos **cadeias de caracteres**.

-	**Inteiro ou (int):** número inteiro. Ex.: 10 ou 50.
-	**Real (float):** número real. Ex.: 10.5 ou 0.8.
-	**Caractere ou Cadeia (string ou char):** número, letras, palavras e/ou outros símbolos. Ex.: "A" ou "abc123" ou "*  é um asterisco.". Tenha sempre em mente que valores do tipo caractere ou cadeia de caracteres são representados entre aspas.
-	**Lógico (bool):** verdadeiro ou falso, sim ou não, 1 ou 0, true ou false.

## Exercícios

**1.	Informe o tipo de variável adequado para cada item abaixo:**

* a)	Idade de uma pessoa
* b)	Valor de uma conta de luz
* c)	Nome de um cliente
* d)	Estado de uma lâmpada (acesa/apagada)
* e)	Senha de acesso ao Facebook
* f)	Quantidade de litros de combustível abastecidos em um posto
* g)	Situação de uma determinada fatura (paga/não paga)
* h)	Média final de um aluno

## Operadores Aritméticos

-	**Soma (+):**				`1 + 3`
-	**Subtração (-):**				`5 – 4`
-	**Multiplicação (*):**			`8 * 8`
-	**Divisão (/):**				`40 / 5`
-	**Resto/Módulo (%):**			`20 % 3`
-	**Potenciação (\*\* ou ^):**		`2 ^ 2`

## Operadores Relacionais

-	**Igual (==)**
-	**Diferente (<> ou !=)**
-	**Maior que (>)**
-	**Menor que (<)**
-	**Maior ou igual (>=)**
-	**Menor ou igual (<=)**

## Operadores Lógicos

-	Conjunção/E (&& ou and)
-	Disjunção/OU (|| ou or)
-	Negação/NÃO (! ou not)

## Tabela verdade
![alt text](images/tabela-verdade1.png "Logo Title Text 1")

## Exercícios

## Precedência de operadores
1.	Parênteses e funções
2.	Potência e resto
3.	Multiplicação e divisão
4.	Adição e subtração
5.	Operadores relacionais
6.	Operadores lógicos

Quando operadores de mesma prioridade se chocam, a operação mais à esquerda prevalece sobre as demais. Ex.:

```
3 * 4 / 3
12 / 3
4
```

```
3 + 4 * 9
3 + 36
39
```

```
(3 + 4) * 9
7 * 9
63
```

Prioridade do operador de multiplicação sobre o de soma
Prioridade dos parênteses sobre o operador de multiplicação

Precedência de operadores

```
10 < 9 e 6 + 3 > 10
10 < 9 e 9 > 10
F e F
F
```

Prioridade do operador de soma sobre os operadores relacionais, e prioridade dos operadores relacionais sobre o operador lógico.
Para facilitar, isole as expressões que estão antes e após o operador lógico, resolva-as e só então compare seus resultados através do operador lógico.

## Exercícios
1.	Indique o resultado das expressões seguindo as regras de precedência dos operadores.

a)	`2 + 3 - 5 * 8 / 4`
b)	`7 * 4 / 2 + 9 - 6`
c)	`(4 + 2) * 3 / 4`
d)	`7 > 2 e 3 -5 < 8`
e)	`8 > 12 e 5 < 3 + 4`

## Comandos de entrada

Comandos de entrada são os responsáveis por receber uma informação do usuário. Ex.: leia, escute, ouça, receba.
```
leia(nome)
```
Quando se trata de linguagens de programação, os comandos costumam ter um par de parênteses logo após seu nome, onde serão informadas opções para sua execução. Neste exemplo, o valor lido é armazenado na variável nome.

## Comandos de saída

Comandos de saída são os responsáveis por enviar uma informação ao usuário. Ex.: escreva, imprima, mostre, exiba.
```
escreva(“Olá, mundo!”)
```
Neste exemplo, o comando `escreva()` irá exibir na tela o texto `Olá, mundo!`.

## Referências Bibliográficas
- LOPES, Anita. GARCIA, Guto. **Introdução à programação – 500 algoritmos resolvidos**. Rio de Janeiro: Elsevier, 2002 - 15ª Tiragem.
