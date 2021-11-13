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
    escreva((a>b) e (b<>a)) <i>//TRUE - porque as duas operações são verdadeiras</i>
    escreva((a/b = 2) ou (a/b = 3)) <i>//TRUE - porque uma das operações é verdadeira</i>
    escreva ((a=b) ou (b>=10)) <i>// FALSE - porque as duas operações estão incorretas</i>
fimAlgoritmo
</code>
</pre>

### Ordem de Precedência

<img src="img/ordem-precedencia.png">
<a href="https://youtu.be/Ig4QZNpVZYs?t=1000" target="_blank">Print tirado dessa vídeoaula</a>

### Exemplo de Código com todas as Operações

<pre>
<code>
algoritmo "temperatura"
var
     t1, t2, t3: real
     geral: logico
inicio
      escreval("Qual era a temperatura de manhã? ")
      leia(t1)
      escreval("Qual era a temperatura de tarde? ")
      leia(t2)
      escreval("Qual era a temperatura de noite? ")
      leia(t3)
      geral <- (t1>15) e (t2>20) e (t3>15)
      escreva("Hoje o dia estava quente? ", geral)
fimalgoritmo
</code>
</pre>

#### Algorítmo Calculador de Idade

<pre>
<code>
algoritmo "minha-idade"
var
   anoAtual, anoNascimento, idade: inteiro
inicio
      escreva("Em que ano estamos? ")
      leia (anoAtual)
      escreva ("Em que ano eu nasci? ")
      leia (anoNascimento)
      idade <- (anoAtual - anoNascimento)
      escreva("Então a minha idade é ", idade ,"!")
fimalgoritmo
</code>
</pre>

<strong>Dica de ouro:</strong> uma ótima ferramenta para práticar algorítmos de forma dinâmica e animada é o <strong><a href="https://scratch.mit.edu/download">Scratch</a></strong>.

#### Algorítmo Conversor de Reais em Dollares

<pre>
<code>
algoritmo "conversor-dollar"
var
   valorDollar, quantiaReais, quantiaPossivel: real
inicio
      escreva("Vou para os Estados Unidos. Quanto o dollar está valendo hoje? ")
      leia (valorDollar)
      escreva ("Quantos reais eu tenho? ")
      leia (quantiaReais)
      quantiaPossivel <- quantiaReais  / valorDollar
      escreva("Então eu consigo comprar US$ " , quantiaPossivel , ".")
fimalgoritmo
</code>
</pre>

#### Algorítmo Conversor de Temperatura

<pre>
<code>
algoritmo "conversor-temperatura"
var
   temperaturaF, temperaturaC: real
inicio
      escreva("A temperatura local está quantos graus em fahrenheit? ")
      leia (temperaturaF)
      temperaturaC <- (temperaturaF - 32) / 1.8
      escreva ("Então aqui está ",temperaturaC:4:1," graus em celsius.")
fimalgoritmo
</code>
</pre>

#### Algorítmo de Cálculo de Taxa de Importação

<pre>
<code>
algoritmo "taxa-importacao"
var
   valorObjeto, taxa, valorTaxado: real
inicio
      escreva("Quanto custa o objeto que comprei?" )
      leia (valorObjeto)
      escreva("Qual é a taxa de importação?" )
      leia(taxa)
      valorTaxado <- (valorObjeto * taxa) / 100
      escreva ("Então eu pagarei ",valorTaxado:5:2,".")
fimalgoritmo
</code>
</pre>

#### Algorítmo Calculador de Parcelas de Empréstimo

<pre>
<code>
algoritmo "emprestimo"
var
   taxa, emprestimo, valorParcelado: real
   parcelas: inteiro
inicio
      escreva("Qual é a taxa de juros para empréstimos nesse banco? ")
      leia(taxa)
      escreva("Quanto você precisa de empréstimo? R$ ")
      leia (emprestimo)
      escreva("Em quantas parcelas você deseja pagar? ")
      leia(parcelas)
      valorParcelado <- (emprestimo + ((emprestimo * taxa)) / 100) / parcelas
      escreva ("Então você pagará ",parcelas," parcelas de R$ ",valorParcelado,".")
fimalgoritmo
</code>
</pre>

## Estruturas Condicionais

As estruturas conficionais são baseadas no fluxo: condição => expressão => resultado. Utilizamos os termos <strong>SE</strong> e <strong>SENÃO</strong> para abrir a condição, logo depois definimos ela através de uma expressão e, com isso, programamos o resultado. Exemplos:

#### Estrutura Simples (SE / IF)

<i>Se eu tiver dinheiro, então comprarei um carro."</i>

O algorítmo dessa expressão seria assim:

<pre>
<code>
algoritmo "se"
var
   resposta: caractere
inicio
    escreva("Eu tenho muito dinheiro? S/N? ")
    leia(resposta)
    se(resposta = "S") entao
        escreva("Então comprarei um carro.")
    fimse
fimalgoritmo
</code>
</pre>

#### Estrutura Composta (SE SENÃO / IF ELSE)

Agora um pouco diferente:

<i>Se eu tiver dinheiro, então comprarei um carro. Senão tiver, comprarei uma bicicleta"</i>

O algorítmo dessa expressão seria assim:

<pre>
<code>
algoritmo "se"
var
   resposta: caractere
inicio
    escreva("Eu tenho muito dinheiro? S/N? ")
    leia(resposta)
    se(resposta = "S") entao
        escreva("Então comprarei um carro.")
    senao
        escreva("Então comprarei uma bicicleta.")
    fimse
fimalgoritmo
</code>
</pre>

### Exemplos de Estruturas Condicionais

#### Par ou Ímpar?

<pre>
<code>
algoritmo "par-impar"
var
    numero: inteiro
inicio
    escreva("Digite um número: ")
    leia(numero)
    se(numero % 2 = 0) entao
        escreval("O número ",numero," é par.")
    senao
        escreval("O número ",numero," é ímpar.")
    fimse
fimalgoritmo
</code>
</pre>

#### Cálculo de IMC

<pre>
<code>
algoritmo "calculo-imc"
var
   altura, massa, imc: real
inicio
      escreva("Qual é sua altura em metros? ")
      leia(altura)
      escreva("Qual é sua massa em kg? ")
      leia(massa)
      imc <- massa / (altura ^ 2)
      se((imc > 18.5) e (imc < 25)) entao
           escreval("O seu IMC é de ",imc:2:1,". Você está no peso ideal.")
      senao
           escreval("O seu IMC é de ",imc:2:1,". Você não está no peso ideal.")
      fimse
fimalgoritmo
</pre>
</code>

#### Habilitação: Apto ou Inapto?

<pre>
<code>
algoritmo "cnh"
var
   anoAtual, anoNascimento, idade: inteiro
inicio
      escreval("--------------------------")
      escreval(" DEPARTAMENTO DE TRANSITO")
      escreval("--------------------------")
      escreva("Ano Atual (yyyy): ")
      leia(anoAtual)
      escreva("Ano de Nascimento (yyyy): ")
      leia(anoNascimento)
      idade <- anoAtual - anoNascimento
      escreval(" ")
      escreval("----------STATUS----------")
      escreval(" IDADE: ",idade," ANOS")
      se(idade >= 18) entao
           escreva(" APTO A TIRAR CARTEIRA")
      senao
           escreval(" INAPTO A TIRAR CARTEIRA")
      fimSe
      escreva("--------------------------")
fimalgoritmo
</pre>
</code>

#### Aluno Aprovado ou Reprovado?

<pre>
<code>
algoritmo "nota"
var
   nota1, nota2, media: real
inicio
      escreva("Primeira Nota: ")
      leia(nota1)
      escreva("Segunda Nota: ")
      leia(nota2)
      media <- (nota1 + nota2) / 2
      escreval(" MEDIA: ",media:2:1)
      se(media >= 7) entao
           escreval(" ALUNO APROVADO")
      senao
           escreval(" ALUNO REPROVADO")
      fimSe
fimalgoritmo
</pre>
</code>

### Condicionais Aninhadas

Essas condicionais são foramdas por mais de uma condição, mais de um SE.

<pre>
<code>
algoritmo "nota"
var
    nota1, nota2, media: real
inicio
    escreva("Primeira Nota: ")
    leia(nota1)
    escreva("Segunda Nota: ")
    leia(nota2)
    media <- (nota1 + nota2) / 2
    escreval(" MEDIA: ",media:2:1)
    se(media >= 7) entao
        escreval(" ALUNO APROVADO")
    senao
        se (media < 7) e (media > 4) entao
            escreval(" ALUNO EM RECUPERAÇÃO")
        senao
            escreval(" ALUNO REPROVADO")
        fimSe
    fimSe
fimalgoritmo
</code
</pre>

