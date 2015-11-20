# workshop-swift-free


#Swift Free
![](http://i68.tinypic.com/25ur7nt.png) 
![Logo do curso de Swift básico](http://i67.tinypic.com/2i9rp5v.png)

# Aulas


# Ementa


* [O Curso](#curso)
    * <b>[Modúlo I](#Modúlo)</b>
    * [A linguagem Swift](#a-linguagem-swift)
    * [Custo](#custo)
    * [Variáveis, uso de opcionais](#variáveis)
    * [Constantes](#constantes)
    * [Operadores](#operadores)
    * [String](#string)
    * [Inteiro e flutuantes](#inteiro-flutuantes-e-boolean)
    * [Convertendo tipos](#convertendo-tipos-inteiros-em-double)
    * [Inferência de tipo](#inferência-de-tipo)
    * <b>[Modúlo II](#Modúlo)</b>
    * [Array](#array)
    * [Dicionário](#dicionário)
    * [Controle de fluxo](#controle-de-fluxo)
    * [Tuplas](#tuplas)
   *  [Funções](#funções)
   *  [Enumeração](#enumeração)
   * <b>[Modúlo III](#Modúlo)</b>
   *  [Classes](#classes-e-objetos)
   *  [Herança](#herança)
   *  [Protocolos](#protocolos)
   *  [Estruturas](#estruturas)
   *  [Extension](#extension)
   *  [Tipo Casting](#tipo-casting)
   * <b>[Modúlo IV](#Modúlo)</b>
   *  [O aplicativo](#o-aplicativo)
   

### Modúlo I

### A linguagem Swift

Criada pela Apple Swift é intuitiva, rápida, moderna e fácil de usar, muito mais fácil que Objective-c.
Swift foi criada e pensada para desenvolvimento de aplicativos. É segura, e divertida.

###Curso
Este curso será dividido em 04 módulos cada um com 01 aula e duração de no máximo 1 hora, 1 vez por semana e sem um dia fixo. Você aprenderá os conceitos básicos da linguagem, como variáveis, constantes, funções e etc. Logo após, teremos a segunda parte do curso, onde desenvolveremos um aplicativo OPEN SOURCE que facilitará o aprendizado das crianças com nosso alfabeto. Esperamos que todos possam implementar e compartilhar nosso código, pois a intenção é que o aplicativo seja sempre "OPEN SOURCE" e benefecie a todos. 

###Custo

> De grátis

### Local

**ONLINE** via Youtube.

###E agora... fud** tudo!

![](http://i65.tinypic.com/qo7rmb.jpg)

###Variáveis

Para declarar uma variável em Swift usa-se a palavra-chave var. Ela pode ser do tipo implícito ou explícito.

####Implícitas
####Exemplo:

```swift
var nome = “José” //String
var sobreNome = “Roberto” //String
var x = 10 //Int
```

```swift
var bandaFavorita = "Black Sabbath"
print("Banda: \(bandaFavorita) ")
```


####Explícitas
```swift
var nome: String = “José” //String
var sobreNome: String = “Roberto” //String
```

```swift
var x:Int = 10 //Int
var y:Int = 20 //Int
```

####Variáveis opcionais, um conceito novo

Em Swift as variáveis e constantes podem ou não ter valor nulo, e decidir quando usá-los.

Para ficar mais claro, veja o exemplo:

```swift
var nome: String?//Veja que usamos a interrogação
nome // erro de compilação, pois a variável não foi inicializada

``` 

![](http://i68.tinypic.com/1zwjlud.jpg)

####Não entendi p***a nenhuma!

![](http://i64.tinypic.com/33ldtvm.jpg)

####Opcionais, e o uso da interrogação

Usa-se a interrogação para informar que sua varável é opcional.

Exemplo:

```swift
var nome: String? //Opcional
```

```swift 
//Para que não ocorra o erro, sabendo que você assume o risco de estar nulo, usa-se o sinal de exclamação
```

![](http://i65.tinypic.com/2jca6v4.gif)

####Forçando o desempacotamento (Forced Unwrapping) com o sinal de ! para acessar o valor de uma variável opcional.

```swift
var nome: String! // A exclamação é usado para forçar seu valor quando você tem certeza que sempre terá algum valor
print(“\(nome)”) // Dará erro, pois sua variável não foi inicializado
```


```swift
var nome: String! // A exclamação é usado para  dizer que seu valor estará sempre disponivel, ou que sua variável terá sempre algo a oferecer.
nome = "Cicrano do escambal"
print(“\(nome)”) //Sua variável foi inicializada, logo executa de boa!
```

```swift
var nome: String?
nome = “Fulano”
print(“\(nome!)”) //Executa normalmente, vejam que nesse caso usei a exclamação no momento da impressão, caso contrário não funcionaria
```


####Lógica do if para verificar se o valor é nulo.

```swift
if let dados = nome {//... } else {//...} 
```
####Verifica se "dados" retorna algo de "nome", caso contrário seu retorno será nulo.

![](http://i64.tinypic.com/15xk38l.png)  

####Com o "if let" é possível evitar o erro em tempo de execução para aquelas variáveis nulas

```swift
var nome: String? //Retorna nil

//Agora quando faço o teste com if, o retorno é nulo pois "nome" não foi inicializada 
```

```swift
if let dados = nome {
    print(dados)
}

else {
    print("nulo")
}

```


![](http://i65.tinypic.com/2ijq4io.jpg)

####Exemplo:

```swift
var xy:String = "De boa na Lagoa!" // valor inicializado
```

```swift
var xy:Int = 30 // valor inicializado
```

###Constantes

Para declarar uma constante em Swift deve-se usar a palavra reservada let e seu valor não pode ser alterado. 


```swift
let x =  "x"
x = "y" // Erro, pois seu valor não pode ser alterado
```

```swift
let cpfDoCliente =  777222555666
print("\(cpfDoCliente)") //Ocorrerá tudo normalmente, pois seu valor não foi alterado
```


```swift
//Uso explicito  do tipo da variável
let telemarketing:String =  "Atendente surdo"
print("\(telemarketing)") //Ocorrerá tudo normalmente, pois seu valor não foi alterado

```

![](http://i66.tinypic.com/35n3b0i.gif)


###Operadores 


![](http://i63.tinypic.com/inr5ee.jpg)


Operadores são símbolos e agregam, alteram ou combinam valores, também podem somar, dividir ou subtrair.

###Operadores aritméticos

####*, +, - e  / 

####Operador de soma

####Exemplo:

```swift
//Uso do operador "+" para somar
var c =  120
var z = 120
var result = c + z
print ("\(result)")
```


####Operador de subtração

####Exemplo:

```swift
//Uso do operador "-" para subtrair

var x =  10
var y = 0
var result = x - y
print ("\(result)")
```

####Operador de multiplicação

####Exemplo:

```swift
//Uso do operador "*" para multiplicar

var livrosBonsDeNietzsche = 10 // Muito mais do que isso
var livrosRuinsDeNietzsche = 0
var result = livrosBonsDeNietzsche * livrosRuinsDeNietzsche
print ("\(result)")// resultado em zero
```


####Operador de divisão

####Exemplo:

```swift
var cuboMagico = 100 
var numeroQualquer = 2
var result = cuboMagico / numeroQualquer
print ("\(result)")// resultado em 50
```

####Operadores de comparação


####Exemplo:

####==, !=, >, <, >= e <= 

```swift
//Uso do sinal de "==" para comparar valores

var macarrao =  "macarrão"
var arroz = "arroz"

if macarrao == arroz {
  print("Alimentos iguais")
}
else {
  print("Alimentos diferentes")
}
```

####Operador !=

####Exemplo:
```swift
//Uso do sinal de "!=" para dizer que não é igual a 

  var numeroMágico = 9

  if numeroMágico != 0 {
    print("9")
  }
  else {
    print("Errado, você viajou na maionese")
  }
```

####Operador >

Maior que

####Exemplo:

```swift

var primeiro_numero =  20
var segundo_numero = 10

if  primeiro_numero > segundo_numero  {
  print("Rodou no if... \(primeiro_numero)")
}
else {
   print("Rodou no else... \(segundo_numero)")
}
```

####Operador <

Menor que

####Exemplo:
```swift
//Uso do sinal de "<"  para comparar se um número é menor que o outro
var notaDoMercado = 20

if notaDoMercado < 10 {
  print("Compras baratas!")
}
else {
  print("Compras caras!")
}
```
####Operador >= 

Maior ou igual a

```swift

####Exemplo:

var x = 220

if x >= 430 {
  print("\(x)")
}


else {
  print("Errou")
}
```
#### Operador <=

Menor igual

####Exemplo:

Menor ou igual a

```swift

var carroDoAno = 200.000
var carroMuitoCaro = "Carro muito carro"

if carroDoAno <= 200.000 {
  print("\(carroDoAno)")
}

else {
  print("\(carroMuitoCaro)")
}

```


###Operador de incremento e decremento

####Incremento

Significa acréscimo. É quando aumentamos o valor de sua variável. Em Swift utilizamos o operador ++

####Exemplo:


```swift

var a = 10// 
++a //Imprime 11, somou + 1 e tem agora o valor de 11 

```

###Decremento

O contrário de incremento. Ocorre quando diminuimos o valor de sua variável. Em Swift utilizamos o operador --
####Exemplo:

```swift
var a = 5 
--a // Imprime 4, e diminuiu em 1

```

###Ternário

Significa avaliar se true ou false, é uma maneira mais eficiente e rápido comparar as variáveis

####Exemplo:

```swift
//Sintaxe:
pergunta? verdadeiro: falso
```

```swift
var seuPaulo = "Chato para cara**o!"
seuPaulo == "Chato para cara**o!" ? "É verdade" : "É mentira"
//O exemplo imprime é verdade
```

```swift
var primeiro_numero = 10
var segundo_numero = 11
primeiro_numero == 11 ? primeiro_numero : segundo_numero
//O exemplo a seguir imprime 11
```

####Operadores lógicos

!, &&, ||   

####Operador lógico ! 

Inverte o boolean, se é "true" retorna "false" e vice-versa

####Exemplo:

```swift
var x = true
if !x {
  print (x)
} 

else {
  print ("false")
}

```

![](http://i67.tinypic.com/2ce4rkl.jpg)

####Operador lógico && 

Operador e

####Exemplo:

```swift
var x = 20
if x > 1 && y > 2 { //Se x e y forem maiores que 1 e 2
  print ("Show...")
} 


```
####Operador lógico ||

Significa ou

####Exemplo:

```swift

var x = 20

if x  > 3 || x < 15 {

  print("Ok") 

}

```


###String 
![](http://i67.tinypic.com/10nzs75.jpg)

Conjunto ou cadeia de carateres que formam texto


####Exemplo:

```swift

var textoDoDia = "Noticia da manhã"
print("\(textoDoDia)") // percebeu o uso do "\(variavel)"... isso é o que chamamos de interpolação de strings, e será visto mais a adiante

```

####Inserindo um caracter

```swift

//Inserindo com o metódo insert

var hello = "Hello"// Gostaria de acrescentar uma exclamação ao final da palavra
hello.insert("!", atIndex: hello.endIndex) // O resultado é: Hello!
//O metódo insert acrescenta um caracter a palavra
```

####Removendo com o metódo removeAtIndex
  
```swift
var saudacao = "saudaçãoo"
saudacao.removeAtIndex(saudacao.endIndex.predecessor()) //Remove o último caracter da palavra
print("\(saudacao)") //imprime saudação 
```


####Concatenando strings

####Exemplo:

```swift
var diaRuim = "Dia muito ruim "
var diaPessimo = "ou pior, está péssimo"
var resultado = diaRuim + diaPessimo
print("\(resultado)") 
```

####Interpolação de strings

Significa combinar variáveis, constantes ou expressões. Basta inserir as variáveis, constantes ou expressões dentro de "\ ()"

####Exemplo:

```swift

var pais = "Brasil"
var situacao = "país que mais se cobra imposto no mundo!"
print ("País: \(pais), \(situacao)")
```


```swift
//Ou assim 

var numero_doze = 12
var numero_setenta = 70
var soma = numero_doze + numero_setenta
print ("\(soma)")
```


###Inteiro, flutuantes e boolean

####Inteiros

####Exemplo:

```swift

var x:Int = 300
```
####Flutuantes

Tanto o float e o double são flutuantes, a diferença é que float  para número de 32 bits com precisão de 6 dígitos e double para número de 64 bits com precisão de 15 dígitos

####Exemplo:

```Swift
//Float
var x: Float = 300.0123456
print(x) // 300.012

//Double
var y: Double = 300.0123456
print(y) // 300.0123456
```

####Boolean

Possue dois tipos de valores, true ou false

####Exemplo:

```swift
var verdadeiro = true

if verdadeiro {
  print("verdadeiro")
}

else {
  print("falso")
}

```

####Convertendo tipos inteiros em double

```swift

var numeroInteiro = 20
var numeroDouble = 20.00
var soma = numeroInteiro + numeroDouble
print("\(soma)") //Erro, pois numeroInteiro possui número inteiro e ao somar com numeroDouble, o xcode não vai compilar
```

```swift

//Experimente fazer dessa forma
var soma = Double (numeroInteiro) + numeroDouble
print("\(soma)")// roda de boa!
```

###Inferência de tipo

Quando falamos em inferência, dizemos que swift deduz seu tipo, ou seja não é preciso necessariamente declarar seu tipo

####Exemplo:

```swift
var cachorroDaVizinha = “Late pra caramba!” //essa é uma String mas em Swift não precisa necessariamente declarar que é uma string
```
```swift

var cachorroDaVizinha:String = “Late pra caramba!” //essa é uma String e declaramos seu tipo string
```


###Modúlo II

###Array
Como em outras linguagens de programação, arrays são coleções de índices ordenados

####Exemplo:

```swift

//Criando um array vazio
var arrayVazio = [Int]()

//Acrescentando ao array
var arrayFromHell = [Int]()
arrayFromHell.append(3) //Imprime 3

```

```swift
//Iterando um array com o for in
var arrayFromHell= [20,30,50]
for a in arrayFromHell {
  print("\(a)")
}

```

####Acessando um array

```swift
var arrayVazio = ["Carro","Moto"]
print(" São \(arrayVazio.count) elementos")// O metódo count, contabiliza os elementos que o array contém
```
#### O metódo append()
```swift

//Modificando o array com o metódo append
var array = ["Chocolate", "Pão"]
array.append ("Biscoito")
print(array) //["Chocolate", "Pão", "Biscoito"]
```

###Dicionário

Dicionários, também são coleções e possuem basicamente chave e valor 

####Exemplo:


```swift

//Sintaxe
[chave 1: valor 1, chave 2: valor 2]

```

####Array simples

```swift

var arrayFilhoDaMae = ["Rockao": "Jimi Hendrix", "Lanche": "hanburgue"]
print ("\(arrayFilhoDaMae)") //Imprime  ["Rockao:" ,"Jimi Hendrix","Lanche: ","hanburgue"]
```

####Como acrescentar um novo indice ao dicionário

```swift

arrayFilhoDaMae ["Jantar"] = "Feijão"
print ("\(arrayFilhoDaMae)") //Imprime ["Rockao": "Jimi Hendrix", "Jantar": "Feijão", "Lanche": "hanburgue"]

```

```swift

//Exemplo de como mudar o valor de um indice em um dicionário:

arrayFilhoDaMae ["Rockao"] = "The who"
print ("\(arrayFilhoDaMae)") //Imprime ["Rockao": "The who", "Jantar": "Feijão", "Lanche": "hanburgue"]

```


###Controle de fluxo

Responsáveis por repetir um determinado pedaço de código até que uma condição expecifica resulte naquilo que esperamos.

####if e else

####Exemplo:


```swift

//Perceba que em Swift, o uso do "if" e "else" não exige necessariamente o uso de parênteses 


var quantidadeDeCarros = 20
if quantidadeDeCarros > 10 {
  // ...
}
else {
  //...
}

```

![](http://i64.tinypic.com/2rx8o4w.png)

###Laço for

####Exemplo:

```swift

//Veja novamente que também no laço "for"  em Swift não exige necessariamente o uso de parênteses

for var x = 0; x < 3; ++x {
  print(x)
}
```

```swift

//Neste exemplo x é multiplicado por 1,2,3,4 e 5

for x in 1...5 {
  print("\(x * 5)")
}
// Resultado impresso
5
10
15
20
25
30
``` 

####Iterando no array com for in:

```swift
var minions = [11,23,44,54,5]
for m in minions {
  print(m) //Imprime todos aqueles
}
```

###Laço While

Executa uma instrução até que a condição seja falsa

####Exemplo:

```swift
var o = 1
while o <= 10 {
  print("\(o)")
  o += 1
}

```

```swift
Variação de "while", realiza uma única passagem atráves do bloco, em seguida, ele continua a repetir o ciclo até que a condição seja falsa
Em outras linguagens usa-se o "do" no lugar do repeat, nesse caso seria "do while" mas aqui em Swift é "repeat while"

var i = 1
repeat { 
  print(i)
  i = i + 1
} while i < 10

```

###Switch

Usado para comparar valores, caso uma das comparações seja verdadeira, o comando é executado

####Exemplo:

```swift


var lacoSwitch = 10
switch lacoSwitch {
  case 2:
    print("1")
  
  case 5:
    print("5")
  
 case 10:
   print("10")// Nesse caso é impresso na tela o numero 10
  
 default:
    print("10")
}
```

###Tuplas

Parecidos com array. As tuplas também agrupam valores e podem ser de qualquer tipo

####Exemplo:

```swift
//Acessando 
var tupla = (3,6)
tupla.0// Imprime 3
```

```swift
//Com o uso de switch
var tuplas = (3,6)

switch tuplas {
  case (1,2):
    print("1,2")
  case (3,6):
    print("3,6")
  default:
    print("3,6")
}  
```


###Funções

Bloco de código que executa uma tarefa expecífica. Usa a palavra chave func

####Exemplo:

```swift
//Função simples e sem retorno
func executar() {
  print("Executando...")
}

executar() // Imprime Executando...
```

```swift
//Função com retorno  
func executar() ->String {
  return "Executando um projeto do cara**o!..."
}  

executar() //Executando um projeto do cara**o!...
```


###Função com parâmetros
Na chamada da função por padrão o nome do primeiro parâmetro é omitido

####Exemplo:
```swift
func calcular(primeiraNota: Int, segundaNota:Int, terceiraNota:Int) ->Int  {
   return (primeiraNota + segundaNota + terceiraNota) / 3
  
}

calcular(7, segundaNota:8, terceiraNota: 10) //Imprime 8

```

###Enumeração
Enumerações são listas, lista de possibilidades de valores a serem usados

####Exemplo:
```swift
//Exemplo simples

  enum planetas {
    case mercurio
    case marte
    case terra
  }  

  var pl = planetas.marte //imprime marte

```

####Enumerações com Switch

```swift

enum planetas {
  case mercurio
  case marte
  case terra
} 

var planeta = planetas.marte

switch planeta {
  case .marte:
    print("Marte") //Imprime Marte
  case .terra:
    print("Terra")
  default:
    print("Marte")
}
```


###Modúlo III

###Classes e Objetos


![](http://i67.tinypic.com/scg7qp.jpg)

Classe, é a unidade que define o comportamento de seus objetos

####Exemplo:




#### Declaração simples de classe

```swift

class Casa {
  
}  
```

#### A classe, as propriedades e os metódos
```swift

class Casa {
  var porta:String = "porta" //propriedade porta
  var janela:String = "janela" //Propriedade janela
  
  //Método interno
  internal func construir () {
    print("construindo casa...")
  }
}
```

####Criando seu objeto e instanciando sua classe

```swift
var c = Casa() //Seu objeto
c.construir() //Chamando um método 

```

####Herança

Quando se herda do seu progenitor. No contexto de programação de computadores, dissemos que o objeto herda caracteristicas de sua classe pai

```swift
 class Apartamento:Casa {
  override func construir() { //Método herdado da classe Casa, a classe pai, veja que usei a palavra chave override reaproveitar o metódo da classe pai
    print("construindo apartamento...")

  }
  
}
```
####Criando seu objeto

```swift
var ap = Apartamento()// Chamando a classe Apartamento
ap.porta = "Porta para apartamento" // Reusando a propriedade porta
ap.janela = "Janela para apartamento" // Reusando a propriedade porta
ap.construir() // Reusando o método construir
```


####Modificadores de acesso 
Aqueles responsáveis pelo comportamento de seus objetos, propriedades, classes e metódos

####Modificador público ou internal

Acessado por qualquer classe ou objeto, esse modificador pode ser colocado também na declaração da classe

```swift  //internal, veja o uso do método internal func utilizar() ```

####Exemplo:

```swift
class Smartphone {
  internal func utilizar () { //Método publico
    print ("Usando o smartphone...")
  }
}  
```


```swift
class Android : Smartphone {
  override func utilizar () { //Veja que utilizei a palavra chave override para reaproveitar o método utilizar
    print ("Usando o Android...")
  }
}  
```


####Modificador privado
Acessado somente por aquela classe, ou seja, ela fica restrita aquele arquivo de origem, esse modificador pode ser colocado também na declaração da classe

####Exemplo:

```swift
class Smartphone {
  private func utilizar () { //Método privado
    print ("Usando o smartphone...")
  }
}   
```


```swift //Erro ```

//Nesse caso não será possível subscrever o metódo pois o metódo utilizar da classe pai é privado
```swift
class Android : Smartphone {
  
  override func utilizar () { //override significa subscrever ao método da classe pai

    print ("Usando o Android...")
  }
}  
```


###Protocolos
Conceito idêntico ao que temos em Java, C#, entre outras linguagens quando se fala em interface. Ou seja, funciona como um acordo onde tenho métodos prontos para serem usados.


####Exemplo:
```swift

protocol Celular {
  func random ()-> Double
}
```

```swift
class Android:Celular {
  func random() -> Double {
    return 1.200
  }
  
  
}
```

```swift
var ce = Android()
print (ce.random()) //Imprime 1.2
```

###Estruturas

![](http://i63.tinypic.com/2afwwa0.jpg)

"Struct" De cara... parecem classes mas diferentimente desses não trabalham com herança. Ambos podem armazenar metódos, propriedades, constantes, variáveis, etc. 
####Exemplo:

```swift

//Struct

struct Casa {
  var porta:Int
  var janela:Int
}

var p = Casa(porta: 2, janela: 3)
}

```

```swift
//Errado, não funcionará pois "struct" não trabalha com herança 

struct Casa:String { 
  var porta:Int
  var janela:Int
}

var p = Casa(porta: 2, janela: 3)

```

###Extension

Adicionam novas funcionalidades a classes, enumerações, estruturas ou tipo de protocolo existente.

####Exemplo:
```swift

//Extendendo o "struct Int"

extension Int { 
  var n: Int {return self * 10}  //N recebe 10
}    

var resultadoDionizico = 10.n //Aqui eu digo que 10 foi multiplicado por 10, já que n recebe 10

```

###Tipo Casting

Uma forma de descobrir a origem do tipo, ou checar uma instância, por exemplo. Usa-se os operadores "is" ou "as".

####Operador is

Checa o tipo da instância, ou retorna true se o que esperamos é verdadeiro ou false caso contrário.

####Exemplo:

```swift
var x: (11,22)

x is Int // Pergunto ao x se ele é do tipo inteiro

//O retorno é true
```


```swift
var x: (11,22)

x is String // Pergunto ao x se ele é do tipo String, o que não é

//O retorno é false
```


####Operador as

Utilizado para indicar o tipo que não estar explicito. Podendo ser usado de duas formas:
Utilizado com o operador !, você força o "casting" e desempacota o objeto, ou utilizando o operador ? que retornará nulo caso você não tenho êxito. Eu sei que vocês não esqueceram do que aprendemos lá trás sobre opcionais.

####Exemplo:

```swift
var cafe =  "Café forte"
cafe as! String // Roda de boa!

```

```Swift

var xicaras = 22
xicaras as? Int //Roda de boa tb

// Experimente fazer o que fiz abaixo

var xicaras:Int!
xicaras as? Int //Nem roda porque xicaras está vazio, nulo, quando uso o sinal de ? estou dizendo que é opcional e assumindo o risco de me retornar nulo

```


### Modúlo IV
###O aplicativo

O aplicativo nasceu para ser open source e tem o propósito de facilitar o entendimento das crianças do nosso alfabeto. Esse mesmo estará disponivel no github.
O app deve ser de fácil entendimento. Tem que ser baseado em exercicios básicos, aqueles ensinados nas escolas para crianças de 4 anos.
Ainda não temos o nome para o aplicativo. Precisamos de ideias para o aplicativo, por isso criei esse repositório <a href = "https://github.com/andersonFaro9/ideiaApp">repositório</a> para que todos coloquem suas ideias e sugestões.

