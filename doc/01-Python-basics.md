# **Python 🐍**
# **Estrutura de Dados**
Em python podemos utilizar diversas estruturas de dados, sendo as principais: Listas, Sets, Dicionários e Tuplas

## Listas
Estrutura de dados que armazena dados em sequência e cada elemento têm sua posição na lista, conhecida como índice. O primeiro elemento sempre é o índice 0.
Podemos utilizar qualquer tipo de dado primitivo seja eles **string, inteiro, float, bool, etc**
Listas são escritas com colchetes.


~~~python
nova_lista = [] # Lista vazia
nova_lista = [1, 2, 3] # Lista de inteiros
nova_lista = [1, 'Hello World!', True] # Lista de diversos tipos
~~~

*Leo, eu posso criar listas dentro de listas?*

 Sim, você pode, e ficaria mais ou menos assim:
~~~python
nova_lista = ['alô', lista1[1, 2, 3], lista2[1.1]]
~~~

## Tuplas

Tuplas são usadas para armazenar múltiplos itens em uma mesma variável (Parece com as listas não?), faz parte de uma coleção ordenada e imutável.
Tuplas são escritas com parênteses
~~~python
nova_tupla = (1, 2, 3) # Tupla de inteiros
nova_tupla = (1, 'opa', 3.3) # Tupla de diversos tipos
~~~

Mas afinal, qual é a diferença entre as listas e tuplas?
Por mais que sejam escritas de maneiras semelhantes, existem momentos que escrever uma tupla é mais eficiente que uma lista. As tuplas podem ser usadas como chave para um dicionários (veremos sobre depois), se tiver que guardar dados que não serão alterados, utilizar uma tupla pode ser melhor, justamente pela sua característica de guardar dados imutáveis, esses dados seriam protegidos de alterações posteriores.

## Dicionários
No Python, os dicionários são coleções de itens desordenados com uma diferença bem grande quando comparados às outras coleções, um elemento dentro de um dicionário possui uma chave atrelada a ele, uma espécie de identificador. É muito utilizado quando queremos armazenar dados de forma organizada e que possuem identificação única (como acontece em bancos de dados). 
Cada valor é atrelado à uma chave, seu identificador.

### Declarando dicionários
~~~python
novo_dicionario = {1: 'João', 2: 'José'}
novo_dicionario = {'nome': 'João', 'sobrenome': 'Silva'}
~~~
### Também podemos usar o método dict(), com o dicionário sendo passado como parâmetro

~~~python
novo_dicionario = dict({{1: 'João', 2: 'José'}})
novo_dicionario = dict({'nome': 'João', 'sobrenome': 'Silva'})
~~~

## Condicionais
Assim como em outras linguagens de programação, python também conta com estrutras condicionais e é bem parecido com o portugol que todos estudamos durante o aprendizado de lógica, por exemplo:
~~~python
n = 10
if n < 10:
    a = 1
elif n > 10:
    a = 2
else:
    a = 0
# Podemos utilizar também o mesmo comando em apenas uma linha:
a = 1 if n < 10 else 2 if n > 10 else 0
~~~
"Traduzindo" para o nosso idioma ficaria mais ou menos assim:
~~~
var = 10

SE var < 10:
    a = 1
SENÃO-SE var > 10:
    a = 2
SENÃO:
    a = 0
~~~
Apesar do código ser auto-explicativo, vou dar uma pincelada sobre a lógica por trás das condições

**IF:** Utilizamos para verificar uma expressão e executar um bloco de código caso a condição seja verdadeira. 
*Posso utilizar a instrução if sozinha?*
Sim, é possível, mas preste também atenção ao " : " no final da instrução.

**ELSE:** Utilizamos para executar um bloco de código, caso o resultado da expressão informada em if seja falso. A expressão **else** só pode ser usada em conjunto com o if, tornando-a impossível de ser utilizada sozinha, mas assim como if também temos que nos atentar ao " : " no final da instrução.

**ELIF:** Este comando é utilizado quando queremos verificar outra expressão, caso a primeira validação seja falsa.


## Loops

Vamos apresentar os famosos "loops" ou laços de repetição em python.
Os laços de repetição (ou laços de iteração) consiste em repetir uma sequência de instruções até que uma condição específica seja atendida. Basicamente, existem dois tipos de laços de repetição em Python: o laço *for* e o laço *while*.

### For:

O laço for é utilizado quando sabemos quantas vezes o bloco será repetido, como por exemplo se desejarmos que o código será executado X números de vezes.
~~~python
for i in range(10):
    print(i, end=" ")
# Será impresso: “0 1 2 3 4 5 6 7 8 9”
~~~

Se observarmos, o número 10 não é mostrado na tela e isso acontece pois em python o contador começa a partir do 0.

### While

Em while nós não sabemos quantas vezes o comando irá se repetir, por isso que *ENQUANTO* ocorre uma instrução, ela se repetirá até que tenhamos o resultado que queremos.

~~~python
contador = 0
while contador < 5:
    print(contador)
    contador = contador + 1 
#Será impresso: 0 1 2 3 4
#Também podemos escrever isso desta forma: contador += 1
~~~

Lembrando que existem diversas possibilidades de usar o *IF* e o *ELSE* junto com essas estruturas também.

### Cláusulas break e continue

Podemos alterar o fluxo de execução de um loop, ***break*** para interromper a execução, ou ***continue*** para avançar para a próxima iteração.

~~~python
for i in range(10):
	if i == 5:
		continue
	if i < 8:
		print(i)
	if i == 8:
		break
#Será impresso: "0 1 2 3 4 6 7"
~~~