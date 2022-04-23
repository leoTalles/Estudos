# Python
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

Leo, eu posso criar listas dentro de listas? Sim, você pode, e ficaria mais ou menos assim:
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

## Loops


