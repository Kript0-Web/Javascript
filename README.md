# Javascript

Javascript é uma linguagem quase obrigatoria para o aprendizado, considerando que quase todo projeto, alguma hora terá que digitar alguma linha em javascrip. Estou desenvolvendo um projeto mobile para meu sistema da faculdade e optei em escrever em react native, porém me senti muito travado e muito isso por conta de não estar familiarizado com a linguagem de javascript. Portando estou comecando um novo estudo, para conhecimentos futuros e terminar o proejto da minha faculdade. Esse documento no github servirá como um armazenanemtno de tudo que aprender, para repassar esse conhecimento e até mesmo revisitalo em algum momento da minha carreira. 

## Oq é 

Basicamente o javascrip é uma linguagem feita para a web, o cliente. Nela é possivel colocar solucoes para incrementar elementos de CSS E HTML. Nos dias atuais essa realidade já não é bem assim, já que a linguagem atualmente consegue programar para o servidor (back-end) com a ajuda do node.js. 

## Tipos de dados e váriaveis 

Como toda linguagens, nós temos as variaveis primitivas sendo elas, number (numeros), string (palavras) e boolean (verdadeiro ou falso). Eu sempre tenho que declarar o tipo de variavel para o meu computador entender o tipo de dado que ele está trabalhando. E como eu declaro uma variável? Podemos usar dois tipos let ou var, os dois sao usados para a mesma coisa ent fica a sua preferencia. Um exemplo seria let nome = lucas. Oq eu esotu fazendo é basicamente, dizer que nome é uma variável e que o nome agora está recebendo a palavra lucas. É assim que os computadores guardam informacoes nas memorias. Outra funcao importante das variavies é a manipulacao das mesmas, ja que eu posso dar uma tratativa para elas. No exemplo do nome lucas, eu poderia usar a variavel nome para mostrar novamente para o usuario oq eu defini.

## Conhecimentos prévios

Toda vez que criarmos um prompt (imput do usuario) ele sempre receberá por padrão uma string, entao caso queiramos receber e manipular dados diferentes disos é preciso converter antes. Ex: let num1 = Number(prompt("Digite o primerio número: ")). Por mais que o vs code já entenda e ja mude pra mim tem algumas momentos que eu preciso forcar o meu programa a usar um tipo especifico de varial, e para isso usaremos o comando parseInt (inteiro) parseFloat. Nota-se que o tipo da variavel tem que ser em maiuscula. Ex let num1 = parseInt(prompt("Digite um numero: "). outra maneira: let num1 = Number.parseInt(prompt("Digite um numero: "). Ele obrigatoriamente tera que armazenar um numero inteiro. E isso serve para que eu obrigue o meu usuario a digitar apenas oq eu quero para evitar problemas de logica ou funcoes especificas. É possivel tbm converter para string e fica assim: alert("o numero digitado foi: " + String((num1)). Outra regrinha, quando criamos uma condição, é preciso colocar o parametro dentro do parenteses. Ex: if (num1 == 1){escrever a trataviva dentro de colchetes}. 

## Tamplate String

É uma maneira de otimizar o uso de varias variaveis em uma frase, ao inves de usar ("meu nome é" + nome + "minha idade é" + idade + "e eu moro em " + cidade), alem de ficar gigante e até uma pouco baguncado, há uma maneira otimizada. Para isso usamos ${} entre o colchetes é o nome da váriavel, e para usar isso também é preciso usar crase `` para formatar dessa maneira, ficando assim:  (`meu nome é ${nome }minha idade é ${idade} e eu moro em ${cidade}`)

## Manipulação de string

Eu posso manipular a minha frase ou so nome da variavel para td minuscula ou maiuscula, tambem posso descobrir o tamanho dessa string e para isso faremos aasim. Para deixar em maiuscula usaremos o comando toUpperCase() entao ficaria tipo `seu nome é ${nome.toUpperCase()}`. Para minuscula é toLowerCase entao ficara `seu nome é ${nome.toLowerCase()}`. E para descobrir o tamanho será length entao ficará `seu nome é ${nome.length()}`. 

## Operadores

### Aritimétricos 

Dentro desse conjunto de operadores existem 6 tipos, sendo eles: 
  + -> Soma
  - -> Subtração
  * -> Multiplicação
  / -> divisão
  % -> resto da divisão
  ** -> elevado

Como na matematica existem uma ordem de precedencia:
1. () Entre parenteses tem maior prioridade, entao td que estiver la dentro será feito primeiro
2. ** Elevado
3. * / %
4. + -
  
## Auto_atribuições

É o método de substiuir o valor de uma variavel por um novo valor. Ex: let num = 3 (esotu dizendo que num está recebendo o valor de 3)
                                                                       num = num + 4 (3 + 4)
                                                                       alert(num) agora vai exibir o resultado 7, pois o 3 foi substituido pelo soma dos dois numero                                                                        e agora passa a receber o novo valor da soma. 
Simplicação é um método de encurtar variveis que serao usadas para a própria. Entao a nova versao seria num += 4. Ele está pegando a váriavel num e ja somando com 4, já que eu escreveria num = num + 4 eu só reduzi o tamanho da escrita. E isto serve para todas as operacoes, desde que use a propria variavel para fazer isso, entao num += x + 4 nao vai dar certo pq estou colocando outra variavel, so serve se receber a própria váriavel. 

### Relacioanis

Para os valores relacionais serao sempre do tipo booleano (verdadeiro ou falso), e dentre eles são:
> -> maior
< -> menor
>= -> maior ou igual
<= -> menor ou igual
== -> igual
!= -> diferente
=== -> exatamente igual, tanto em valor como tipo de variavel, se eu tiver q 5 == "5" o javascript entende que sim eles são iguais, pois sao de mesma grandeza. Agora 5 === "5" é falso, ja que eles sao iguais em grandeza, mas nao em tipo de dados, um é numero outro é string. Para ser verdadeiro eles tem que ter o mesmo numero e mesmo tipo. Isso é conhecido como operador de identidade.

 ### Operadores lógicos

Para os valores relacionais serao sempre do tipo booleano (verdadeiro ou falso), e dentre eles são:
! -> significa diferente
&& -> segnifica que tem que ter duas afirmacoes para ser verdadeiro, ex: quero uma caneta azul e preta, obrigatoriamente tem que ser uma azul e uma preta, caso eu traga uma delas ou nenhuma delas entao sera falso. É como se fosse um crianca mimadam, nao adinta ganhar um ainda quer o outro.
|| -> significa que apenas uma das afirmacoes tem que ser verdadeira. Ex: Quero uma caneta azul ou preta, qualquer uma delas que eu trouxer vai ta bom de mais, se trazer as duas melhor ainda, mas eu so exigi uma ou outra. 
