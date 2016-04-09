# Apostila de Lógica de Programação

A **Lógica de Programação** é a técnica de encadear pensamentos para atingir determinado objetivo por meio de um computador ou outro sistema programável.

Antes de começarmos a programar, é necessário compreender novos conceitos e até rever alguns dos já vistos nas aulas de Matemática.

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
- Algumas linguagens de programação diferenciam letras maiúsculas de letras minúsculas, logo: `Nome` pode ser diferente de `nome`
- Variáveis cujo nome seja um substantivo composto, como "data de nascimento", **podem** ser nomeadas com o padrão camelCase: `dataDeNascimento`. Este padrão define que todas as palavras após a primeira devem começar com letra maiúscula. Outra alternativa é utilizar um traço inferior (`_`), ou underline, entre cada palavra: `data_de_nascimento`.


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

### Exercícios

**1.	Informe o tipo de variável adequado para cada item abaixo:**

* a)	Idade de uma pessoa
* b)	Valor de uma conta de luz
* c)	Nome de um cliente
* d)	Estado de uma lâmpada (acesa/apagada)
* e)	Senha de acesso ao Facebook
* f)	Quantidade de litros de combustível abastecidos em um posto
* g)	Situação de uma determinada fatura (paga/não paga)
* h)	Média final de um aluno

## Operadores


### Operadores Aritméticos

-	**Soma (+):** `1 + 3`
-	**Subtração (-):** `5 – 4`
-	**Multiplicação (*):** `8 * 8`
-	**Divisão (/):** `40 / 5`
-	**Resto/Módulo (%):** `20 % 3`
-	**Potenciação (\*\* ou ^):** `2 ^ 2`

### Operadores Relacionais

-	**Igual (==):** `5 == 5`
-	**Diferente (<> ou !=):** `8 != 80`
-	**Maior que (>):** `12 > 11`
-	**Menor que (<):** `11 < 12`
-	**Maior ou igual (>=):** `18 >= 17`
-	**Menor ou igual (<=):** `16 <= 16`

### Operadores Lógicos

-	**E/Conjunção (&& ou and):** `5 == 5 && 9 > 7`
-	**OU/Disjunção (|| ou or):** `5 > 3 || 7 >= 1`
-	**NÃO/Negação (! ou not):** `!(3 > 2) == falso`

## Tabela verdade
Uma tabela verdade é uma tabela utilizada em Lógica para verificar se uma expressão é verdadeira ou falsa.

### Operadores "e" e "ou"

No exemplo a seguir, temos a tabela verdade dos operadores lógicos `e` e `ou`. Observe que as variáveis `X` e `Y` representam expressões que podem ser verdadeiras ou falsas de forma independente.

![alt text](imagens/tabela-verdade1.png "Tabela Verdade 1")

Para compreender como se dá a construção dessa tabela verdade, podemos nos fazer estas duas perguntas:

- `X` e `Y` são verdadeiros?
- `X` ou `Y` são verdadeiros?

Ao questionar se `X` e `Y` são verdadeiros, questionamos se ambos são verdadeiros. Ou seja: a expressão `X e Y` só é verdadeira quando `X == verdadeiro` e `Y == verdadeiro`.

O operador `ou` já funciona de maneira diferente. Ao questionarmos se `X` ou `Y` são verdadeiros, questionamos se pelo menos um deles é verdadeiro. Ou seja: a expressão `X ou Y` é verdadeira quando `X == verdadeiro` e `Y == falso`, ou `X == falso` e `Y == verdadeiro`, ou `X == verdadeiro` e `Y == verdadeiro`.

### Operador "não"
O operador `não` é utilizado para negar uma determinada expressão. Ex.: se `X == verdadeiro`, então `não X == falso`; se `X == falso`, então `não X == verdadeiro`.

![alt text](imagens/tabela-verdade2.png "Tabela Verdade 2")

### Exercícios
**1. Complete a seguinte tabela verdade:**

![alt text](imagens/tabela-verdade-exercicios.png "Tabela Verdade - Exercícios")

## Precedência de operadores
A precedência, ou ordem, de operadores é a convenção que indica a ordem em que as operações devem ser realizadas em uma expressão. A lista abaixo descreve a ordem em que os operadores devem ser considerados:

1.	Parênteses e funções
2.	Potência e resto
3.	Multiplicação e divisão
4.	Adição e subtração
5.	Operadores relacionais
6.	Operadores lógicos

No exemplo abaixo, a multiplicação deve ser resolvida antes da soma.
```
3 + 4 * 9
3 + 36
39
```

Neste exemplo, a parte da expressão entre parênteses é resolvida antes da multiplicação.
```
(3 + 4) * 9
7 * 9
63
```

Quando operadores de mesma prioridade se chocam, a operação mais à esquerda prevalece sobre as demais. Ex.:

```
3 * 4 / 3
12 / 3
4
```

Neste exemplo, o operador de soma tem prioridade sobre os operadores relacionais, e os operadores relacionais têm prioridade sobre o operador lógico.
```
10 < 9 e 6 + 3 > 10
10 < 9 e 9 > 10
F e F
F
```
Para facilitar, isole as expressões que estão antes e após o operador lógico, resolva-as e só então compare seus resultados através do operador lógico.

### Exercícios
**1.	Indique o resultado das expressões seguindo as regras de precedência dos operadores.**
- a)    `2 + 3 - 5 * 8 / 4`
- b)	`7 * 4 / 2 + 9 - 6`
- c)	`(4 + 2) * 3 / 4`
- d)	`7 > 2 e 3 -5 < 8`
- e)	`8 > 12 e 5 < 3 + 4`

## Fluxo básico de um programa



### Comandos de entrada

Comandos de entrada são os responsáveis por receber uma informação do usuário. Ex.: leia, escute, ouça, receba.
```
leia(nome)
```
Quando se trata de linguagens de programação, os comandos costumam ter um par de parênteses logo após seu nome, onde serão informadas opções para sua execução. Neste exemplo, o valor lido pelo comando `leia()` é armazenado na variável `nome`.

### Comandos de saída

Comandos de saída são os responsáveis por enviar uma informação ao usuário. Ex.: escreva, imprima, mostre, exiba.
```
escreva(“Olá, mundo!”)
```
Neste exemplo, o comando `escreva()` irá exibir na tela o texto `Olá, mundo!`.

### Um básico exemplo de entrada, processamento e saída
```
leia(a)
leia(b)
c = a + b
escreva(c)
```

## Referências Bibliográficas
- LOPES, Anita. GARCIA, Guto. **Introdução à programação – 500 algoritmos resolvidos**. Rio de Janeiro: Elsevier, 2002 - 15ª Tiragem.
