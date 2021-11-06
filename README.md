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