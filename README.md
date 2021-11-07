### O que são algorítmos?

Os algorítmos são uma sequência de ações executadas para a solução de um problema. Como por exemplo:

<pre>
<code>
algoritmo atravessarRua
    olhar para a direita
    olhar para a esquerda
    se estiver vindo carro
        não atravesse
    senão
        atravesse
    fim-se
fim-algoritmo
</code>
</pre>

### Algorítmos computacionais

Os algorítmos computacionais são desenvolvidos através de 3 fases:

<ul>
    <li>Lógica de programação</li>
    <li>Linguagem de programação</li>
    <li>Sistema completo</li>
</ul>

A lógica de programação é estruturada através de uma linguagem para construir um sistema completo.

### Portugol

O portugol é uma maneira de representar a lógica de programação para converter para uma linguagem.

Através do programa <strong>VisuAlg</strong>, foi possível desenvolver esse meu primeiro código:

<pre>
<code>
algoritmo "primeiro-comando"
var
inicio
    Escreva ("Ola, mundo!")
fimalgoritmo
</code>
</pre>

Como resultado, eu tive a mensagem: <i>Ola, mundo!</i>

### Outros comandos

#### Texto em uma nova linha:

<pre>
<code>
    escreval ("Linha de cima")
    escreva ("Linha de baixo")
</code>
</pre>

<strong>Resultado:</strong>
<i>Linha de cima<br>
Linha de baixo</i>

### Variáveis

#### Identificadores
Os identificadores são as palavras que definem a variável. Devem começar com uma letra e não podem ter símbolos (com exceção do underline (_)) ou espaços, também não podem ter o mesmo nome das palavras reservadas ("inicio", "var", "algoritmo", etc).

<strong>Exemplos:</strong> teste1, nome_teste, algoritmos_saoLegais

#### Tipos Primitivos
<ol>
<li><strong>Inteiro:</strong> 1, 200, -89, 0</li>
<li><strong>Real:</strong> 0.5, 2.75, -35.6</li>
<li><strong>Caractere:</strong> "Teste", "Isso é um texto", "Algoritmos"</li>
<li><strong>Lógico:</strong> verdadeiro, falso</li>

#### Exemplo de atribuição de variável
<pre>
<code>
algoritmo "segundo"
var
    nome: caractere
inicio
    nome <- "Renato"
    escreva ("Olá, o meu nome é " + nome)
fimAlgoritmo
</code>
</pre>

### Comandos de entrada

<pre>
<code>
algoritmo "olaNome"
var
    nome: caractere
inicio
    escreva ("Olá, o seu nome é: )
    leia (nome)
    escreva ("Muito prazer, " + nome)
fimAlgoritmo
</code>
</pre>

<strong>leia</strong> é um comando de entrada<br>
<strong>escreva</strong> é um comando de saída

### Operadores Aritméticos

São operadores aritméticos aqueles que são usados para realizar contas matemáticas, como adição ( + ), subtração ( - ), multiplicação ( * ), divisão ( / ), divisão inteira ( \ ), exponênciação ( ^ ) e resto da divisão ( % ).

Alguns exemplos:

<pre>
<code>
algoritmo
var
    a, b: inteiro
inicio
    a <- 5
    b <- 2
    escreva(a+b) <i>//adição</i>
    escreva(a-b) <i>//subtração</i>
</code>
</pre>

#### Soma de valores

<pre>
<code>
algoritmo "soma"
var
    numero1, numero2, soma: inteiro
inicio
    escreva ("Digite o primeiro número: ")
    leia (numero1)
    escreva ("Digite o segundo número: ")
    leia (numero2)
    soma <- numero1 + numero2
    escreva ("A soma entre ",numero1," e ",numero2," é igual a ", soma)
fimAlgoritmo
</code>
</pre>

#### Exemplo de uma equação em algorítmos
<pre>
<code>
algoritmo "equacao"
var
    resultado: real
inicio
    resultado <- (7 + 3) / 5
    escreva(resultado)
fimAlgoritmo
</code>
</pre>

### Operadores relacionais

Os operadores relacionais são aqueles que determinam se tal operação é verdadeira ou falsa. São eles: maior que ( > ), menor que ( < ), maior ou igual a ( >= ), menor ou igual a ( <= ), igual a ( = ), diferente ( <> ).

Alguns exemplos:

<pre>
<code>
algoritmo
var
    a, b: inteiro
inicio
    a <- 10
    b <- 5
    escreva(a>b) <i>//TRUE</i>
    escreva(a+b=b%2) <i>//FALSE</i>
fimAlgoritmo
</code>
</pre>

### Operadores Lógicos

Os operadores lógicos comparam dois valores e determinam se o resultado é verdadeiro ou falso através dos operadores E e OU.

<pre>
<code>
algoritmo
var
    a, b: inteiro
inicio
    a <- 10
    b <- 5
    escreva((a>b) e (b<a)) <i>//TRUE - porque as duas operações são verdadeiras</i>
    escreva((a/b = 2) ou (a/b = 3)) <i>//TRUE - porque uma das operações é verdadeira</i>
    escreva ((a=b) ou (b>=10)) <i>// FALSE - porque as duas operações estão incorretas</i>
fimAlgoritmo