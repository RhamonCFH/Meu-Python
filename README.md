Python

Anotações python
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
AULA SOBRE INSERÇÃO DE OPERADORES ARITMÉTICOS
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# +, -, /, *, // (DIVISÕES EXATAS, SEM CASAS DECIMAIS)
#Adição, subtração, divisão e multiplicação  

a = 4

b = 4

print(a+b)#adição

print(5-2)#subtração

print(5*2)#multiplicação

print(10/6)#divisão

print(10//6)#divisão exata

print(10%2)#resto da divisão bom para identificar números pares ou ímpares

#Números pares não tem resto, já o impar sim

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Como sugestão de prática, indicamos você a criar um novo script python seguindo as orientações a seguir:

Crie três inputs que receba os três dados abaixo:
-Nome do tipo string

-Altura do tipo Float

-CPF do tipo inteiro

Exiba através de um único print as três informações para o usuário.

nome = input('Nome: ')

altura = float(input('Altura: '))

cpf = int(input('CPF: '))

print('Meu nome é', nome,',tenho ', altura, 'metros de altura', 'e meu cpf é', cpf)

Nome: Rhamon

Altura: 1.84

CPF: 184

Meu nome é Rhamon , tenho  1.84 metros de altura e meu cpf é 184
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Operadores de relação e condição

#Operadores de igualdade

#==, != (iguais e diferentes) = uma vez tem valor de atribuição

#Operadores relacionais ou condicionais

#>, <, <+, >= (Maior que, menor que, menor ou igual e maior ou igual.)
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
#Aplicabilidade nos  códigos

numero = 100==100

print(numero)#quando colocamos para ler, ele lê se a comparação é True or False

print(type(numero))#o type classifica qual a variável trabalhada

numero = 100!=100

print(numero)#False

numero = 100>101#False

print(numero)

numero = 100<101#True

print(numero)

numero = 100>=101#False

print(numero)

numero = 100<=101#True

print(numero)

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
COMANDO If e Else e Elif

#Controle de comando de condição

#Cria uma situação hipotética, pra colocar se  uma condição for atendida

'''O comando if serve para quando o resultado daquele algo seja o desejável e 
o comando Else é pra quando o comando for diferente daquilo , ou não for 
aquele desejável pelo programador.

Else é  a fuga da excessão, quando nenhum deles é atendido.'''

numero = 11

if numero == 10: #True

    print('Este número é igual a 10!')
    
elif numero == 11:

    print('Este número é igual a 11')
    
elif numero == 12:

     print('Este número é igual a 12')
     
elif numero == 13:

     print('Este número é igual a 13')
     
else:

    print('Este número não é igual a nem 10, 11, 12 ou 13!')
    

#Elif é a união entre o if e o else, onde vamos colocar uma condição nova.

#Elif é a excessão sobre o if. Dá diversas condições sobre os outros resultados.

numero = int(input('Digite o número: '))

if numero == 1:

    print('Este número é o correto.')
    
elif numero == 2:

    print('Um pouco abaixo.')
    
elif numero == 3:  

    print('Um pouco mais abaixo.')
    
elif numero == 4:

    print('um pouco bem mais abaixo.')
    
else:

    print('Está bem longe.')
    
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
'''Como sugestão de prática, indicamos você a criar um novo script python seguindo as orientações a seguir:

Crie uma variável número e atribua o valor 15 a ela.

Crie um comando de condição para verificar se ela é == a 15, 

Menor que 15, maior que 15.

Informar através de print a informação para o usuário.'''

numero = int(input('Digite o número: '))

if numero == 15:

    print('Certamente, igual a 15')
    
elif numero < 15:

    print('Certamente você está incorreto.')
    
elif numero > 15:

    print('Equivocadíssimo')
    
else:

    print('Tudo errado mermão')
    
Não precisa colocar Else.
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Comandos de controle de fluxo

(ESSE COMANDO SIGNIFICA O SEGUINTE. Enquanto i for maior ou = a 10, ele vai ser gerado no sistema como i, e ai cada vez que ele é exercido, ele faz ele mais 1. Até chegar a 10.) 

#Controle de fluxo, primeiro comando while = enquanto

'''Fluxo de informações, com uma condição e quantidade de vezes.'''

i = 0

while(i<=10):

    print(i)
    
    i = i+1
    
0

1

2

3

4

5

6

7

8

9

10

while(i<=10):

    print('O loop está rodando...')
    
    i = i+1
    
#ou i+=1

O loop está rodando...

O loop está rodando...

O loop está rodando...

O loop está rodando...

O loop está rodando...

O loop está rodando...

O loop está rodando...

O loop está rodando...

O loop está rodando...

O loop está rodando...

O loop está rodando...

Faz isso por 10 vezes

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
for é usado para mais de um tipo de repetição.

#for faz para um fim específico com mais de um tipo de dados.

for i in 'Python':

    print(i)
    
    #for composto pelo comando, variável contadora, pela estrutura in 
    
    #que vai dizer o que a variável contadora vai executar 
    
    #e aquilo que vai ser contado ou percorrido

num = (1,5,6,7)

for j in num:

     print(j)
     
P

y

t

h

o

n

1

5

6

7
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
#Código voltado para a maneira aleatória

for i in range(10):#for, variável contadora i, in e range que vai fazer o código gerar 10 elementos.

     print(i+1)

print ('-----------------')

for j in range(-10,0,1):

     print(j)
     
     # (de onde começa, o ponto de chegada e a saltar de, no caso de 1 em 1)

-10

-9

-8

-7

-6

-5

-4

-3

-2

-1

for j in range(-10,10,2):

     print(j)
     
-10

-8

-6

-4

-2

0

2

4

6

8

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Como sugestão de prática, indicamos você a criar um novo script python seguindo as orientações a seguir:

#Crie um laço com for in range que imprima os múltiplos de 3 no intervalo entre 0 e 15.

for i in range(0, 16, 3):

    print(i)
    
0

3

6

9

12

15

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
#Duas instruções, Break e Continue , para quebrar ou pausar uma tarefa de código e depois continuar
print('Entrando no laço.....')

for i in range(10):

    print(i)
    
    if(i == 5):
    
        break 
        
print('Saindo do laço...')


Entrando no laço......

0

1

2

3

4

5                 

Saindo do laço...

O break vai servir para quando o comando chegar em 5 contagens, ele deve pausar ali aquela função e não exercer mais do que isso.

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

print('Entrando no laço....')

i = 0

while(i<10):

    i+=1
    
    if(i%2==0):         
    
    continue
    
    print(i)
    
print('Saindo do laço...')

Entrando no laço....

1

3     

5

7

9

Saindo do laço...

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# while ia rodar 10 vezes, porém, está dizendo que sempre que houver número par, ele vai ignorar o número par e vai continuar imprimindo os demais.

#O break para e o continue ignora uma parte do fluxo e continua.

( se o resto da minha divisão por 2 for igual a 0, ou seja um número par, ele deve pausar e continuar. Sem o número par.)

Entrando na gaiola...

1

2

4

5

7

8

10

Saindo da gaiola....

print('Entrando na gaiola...')

i = 0

while(i<10):

    i+=1
    
    if(i%3==0):
    
     continue
     
    print(i)
    
print('Saindo da gaiola....')

 IMPARRRRR
 
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
STRINGS

#Strings- funções e características dessa Estrutura de dados. Tem informações dentro com cadeias de caracteres. A união de chars são strings. ex: char = R, char = H, char = A... etc.

nome = 'Rhamon Hack'

nome2 = 'Rhamon Hack'

nome3 = '''Esta é uma string longa 

contendo informações sobre 

Python'''

nome4 = """Esta é uma string longa 
com aspas dulplas na
Linguagem
Python
"""
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

print(nome)

print(nome2)

print(nome3)

print(nome4)

Rhamon Hack

Rhamon Hack

Esta é uma string longa 

contendo informações sobre 

Python

Esta é uma string longa 

com aspas dulplas na

Linguagem

Python

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
#PROPRIEDADES DAS STRINGS

l = 'lista de letras'

#tamanho da string

tamanho = len(l) #len é a função que nos retorna o tamanho da nossa string, ou seja, a quantidade de caracteres naquele espaço composto por l. no caso, 15.

print(tamanho)

#split da string

lista = l.split(" ")

print(lista) 

#Cria pra gente uma estrutura de dados contendo os pedaços da string selecionada, no caso, l.

#Você usa no (' ') espaço dentro do split aquilo que tem entre os caracteres.

data = '15/09/2021'

tamanhodata = len(data)

print(tamanhodata)

lista2 = data.split('/')

print(lista2)
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
#Propriedade de substituição

#substituir um espaço (caracter da string) por outro.

#Função REPLACE

#print(l.replace('de', 'os'))

print(l.replace('de', 'os'))

print(data.replace('15', '29'))
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
'''Fatiamento e divisão de string

Conceito de indexação- posições que os caracteres ocupam dentro da cadeia.

índices começam do 0. Primeiro caracter ocupa o índice 0, o segundo, índice 1, e assim em diante.
'''
# TEREMOS COMO BASE ESSA INDEXAÇÃO

# Agora podemos começar a fatiar as strings

#Fatiar é utilizar apenas uma parte da string que é interessante para nós.

#Quer apenas o índice 1 daquela string.

#       012345          5 ÍNDICES E 6 CARACTERES

#      -5-4-3-2-1 Podemos fazer com números negativos também. Será ao contrário.

nome = 'python'

nova_string = nome[0:6:2]#Aqui é usado chaves ao invés de colchetes. e coloca o índice que você quer.

print(nova_string)

#Podemos fazer a impressão começando em um local e terminando em outro. é só colocar os : após o primeiro número.

#Mais um :, você coloca a quantidade de caracteres que você quer q sejam saltados.

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

'''Comparação de strings

False

True

True

True

As duas primeiras são óbvias as respostas, mas se for olhar as duas últimas, 
no que o pyhton se baseia para colocá-las como verdadeiras?'''

#Se baseia na Tabela ASCII, cada um desses caracteres são utilizados e possuem um valor. E por isso consegue fazer a comparação.

#Então vamos imprimir a tabela ASCII, vamos fazer um for in range com 122 itens, e imprimir o i como formato de string, + o caracter da tabela ASCII.

print('a' == 'b')

print('b' != 'a')

print('a' > 'X')

print('a' > '1')

for i in range(122):

    print(str(i) + ' - '+chr(i))

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
#Percorrendo a String, usando estruturas como for e while.

nome = 'pyhton'

#percorrer com for

for i in nome:

    print(i)

print('----------------------')
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
#percorrer com while

i = 0

while i<len(nome):

    print(nome[i])
    
    i+=1
    
print('------------------------')

#É como se colocasse (while(i<6), porque tem 6 caracteres. (len - tamanho)

#percorrer com for / enumerate

#uma varável que uma vai assumir um número e a outra um valor.

for x, z in enumerate(nome):

    print(x,z)
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
LISTAS

'''modelos de indexação 0 1 2 3 4 5 .... n'''

nome = 'python' #listas tipos floats, int e str, listas vazias tbm.

lista = [2,3,4,5]

lista2 = [1.5,4.5,6.5]

lista3 = [1,1.5,'número']

lista4 = []

print(lista2[1])


lista = [100,200,300,400,500,600,700,800]

for i in range(len(lista)):

    lista[i]+=1
    
    print(lista[i])
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
FATIAMENTO DE LISTAS

#conceito de indexação 

#        0  1  2

lista = [2,3,4]

#       -3 -2 -1

nova_lista = lista[0:2:2] #intervalo entre eles, o 2 n entra, o último é saltar de quanto em quanto.

print(nova_lista)

lista2 = ['p','y','t', 'h', 'o', 'n']

nova_lista2 = lista2[::-1]#Ele imprime ao contrárioi pq eu não passei de onde eu começo, newm de onde 3eu termino e falei para pular de -1 em -1.(ou seja, valores ao contrário).

print(nova_lista2)

['n', 'o', 'h', 't', 'y', 'p']
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
'''Como sugestão de prática, indicamos você a criar um novo script python seguindo as orientações a seguir:

Crie uma lista abaixo com a seguinte palavra:

“PYTHON”

A lista deve conter as letras separadas e em maiúsculas.

Crie uma nova lista somente com as três últimas letras da palavra “PYTHON”.'''

        #0 1 2 3 4 5
        
lista = ['P', 'Y', 'T' ,'H' ,'O' ,'N']

nova_lista = lista[3:6]

print(nova_lista)
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Inserções, exclusões e outras possibilidades.

animais = ['gato', ' cachorro', 'elefante']

animais.append('galinha')

print(animais)

['gato', ' cachorro', 'elefante', 'galinha']

Galinha adicionada a lista

animais = ['gato', ' cachorro', 'elefante']

animais.append('galinha')#adiciona

print(animais)

animais.insert(0, 'Papagaio')#substitui no local q vc desejar.

print(animais)

animais.pop(0)#remove pelo índice

print(animais)

animais.remove('gato')#tira o elemento também, mas de acordo com o que escreve.

print(animais)

['gato', ' cachorro', 'elefante', 'galinha']

['Papagaio', 'gato', ' cachorro', 'elefante', 'galinha']

['gato', ' cachorro', 'elefante', 'galinha']

[' cachorro', 'elefante', 'galinha']


---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Ordenando:

lista = ['a', 'x', 's', 'w', 'd','a', 'n', 'a']

#reverte a lista lista.reverse()

#ordenar os elementos lista.sort()


for i in range(len(lista)):

    print(lista[i])

l = lista.count('a')#conta a qauntidade de vezes que aquela variável se repetiu.

print(l)

a

x

s

w

d

a

n

a

3

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

'''Como sugestão de prática, indicamos você a criar um novo script python seguindo as orientações a seguir:

Crie uma lista de móveis de uma casa;

Adicione um elemento no final da lista;

Remova um elemento pelo seu índice.'''

lista = ['geladeira', 'fogão', 'armário', 'mesa']

lista.insert(4, 'sofá')

print(lista)

lista.remove('geladeira')

print(lista)

lista.pop(1)

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
'''Tuplas

Estrutura de dados parecida com as listas, mas com mudanças bem perceptíveis, 
não conseguimos alterálas

Lista usamos colchetes, e tuplas parênteses()'''

#PODEMOS TER MUITOS TIPOS DE TUPLAS.

t = tuple('abc') #TUPLAS STRINGS

x = ('python') #TUPLAS STRINGS

x1 = (2,3,4) #TUPLAS INTEIRAS

x2 = (2.5, 1.6, 4.8) #TUPLAS FLOAT

x3 = ('python', 1, 4.5, True) #TUPLAS MISTAS COM STR, INT,FLOAT E BOOLEANA (BOOL)

print(x3)
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
#Se quisermos ver o tipo, colocamos:

print(type(x3)) #<class 'tuple'>
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
"""Operaçõesp possíveis nas tuplas"""

elementos_tupla = ('São Paulo', 'Belo horizonte', 'Teresina' )

print("Teresina" in elementos_tupla)

#True recebemos uma verificação de True ou False. Se fosse outro nome, exemplo, Manaus

print("Manaus" in elementos_tupla)

#False

nomes_tupla = ('José', 'Carlos', 'Maria', 'Pedro', 'Maria', 'Joana', 'Maria')

print(nomes_tupla.count('Maria'))

#Fazemos isso para saber a quantidade de 

#Elementos que possuem dentro daquela operação. No caso o count que 

#é para contar os elementos.

#Resposta : 3

#Quero verfificar o índice do elemento da tupla.

print(nomes_tupla.index('Carlos'))

#Resposta: 1
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
"""Dicionários, podemos defini-los e colocar outras estruturas de dados nele tbm"""

#Colocamos a chave e o valor dela. valor a, chave amor.

#Podemos ter dicionarios de str, int, float e tbm colocar estruturas como tuplas com o valor de uma listas, etc.

dicionario = {'a': "amor", "b":"blue"}

dicionario2 = {1:20, 3:30, 4:30}

dicionario3 = {5.5:50.50, 30.1:30.25}

dicionario4 = {(10,20):['python', 'línguagem', 10]}

print(dicionario)

print(type(dicionario))

#{'a': 'amor', 'b': 'blue'}

#<class 'dict'>
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
"""Novas formas de acesso aos dicionários"""

dicionario = {'a': 'letraA', 'b':'letraB', 'c':'letraC'}

print (dicionario['a'])

print (dicionario['b'])

print (dicionario['c'])

#letraA letraB letraC

#Como não conseguimos encontrar, conseguimos colocar outra mensagem como 'Valor não encontrado

print(dicionario.get('d', 'Valor não encontrado'))

#KeyError: 'd' Valor não encontrado

agenda = {402023032:'José', 21813183920: 'Cristiano', 2128032091: 'Carlos', 2109231120: 'Maria'}

print(agenda)

del(agenda[402023032])

print(agenda)

#{402023032: 'José', 21813183920: 'Cristiano', 2128032091: 'Carlos', 2109231120: 'Maria'}

#{21813183920: 'Cristiano', 2128032091: 'Carlos', 2109231120: 'Maria'}

print(agenda.keys()) 

#Serve para voce imprimir a lista só com as chaves, no caso os númeors e a outra para 
#imprimir só com os valores, no caso, os nomes.

print(agenda.values())

print(len(agenda))# 3

print(agenda.popitem()) #cada popitem que voc~e dá ele retira um elemento

print(agenda)

print(agenda.popitem())

print(agenda)

#(2109231120, 'Maria')

#{21813183920: 'Cristiano', 2128032091: 'Carlos'}

#(2128032091, 'Carlos')

#{21813183920: 'Cristiano'}

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
"""Como sugestão de prática, indicamos você a criar um novo script python seguindo as orientações a seguir:

Crie um dicionário contendo dias da semana sendo dia1, dia2, dia3... as chaves e o dia seu valor. Ex: “dia1”: “domingo”.

Remova dois dos últimos dias da semana.

Remova segunda-feira pela sua chave.

Imprima chaves e valores do dicionário.

Imprima o dicionário final."""
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
dicionario = {'dia1': 'segunda', 'dia2': 'terça', 'dia3': 'quarta', 'dia4': 'quinta', 'dia5': 'sexta'}

print(dicionario)

dicionario.popitem()

print(dicionario)

dicionario.popitem()

print(dicionario)

del(dicionario['dia1'])

print(dicionario)

print(dicionario.keys())

print(dicionario.values())

print(dicionario)

"""{'dia1': 'segunda', 'dia2': 'terça', 'dia3': 'quarta', 'dia4': 'quinta', 'dia5': 'sexta'}

{'dia1': 'segunda', 'dia2': 'terça', 'dia3': 'quarta', 'dia4': 'quinta'}

{'dia1': 'segunda', 'dia2': 'terça', 'dia3': 'quarta'}

{'dia2': 'terça', 'dia3': 'quarta'}

dict_keys(['dia2', 'dia3'])

dict_values(['terça', 'quarta'])

{'dia2': 'terça', 'dia3': 'quarta'}"""

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
"Funções - pode fazer várias ações sem precisar ficar repetindo"

def função():#def = definição de função. O parãmetro está vazio pq por enquanto n tem nenhum parâmetro.

    print('Eu sou uma função!')#Podemos colocar tudo que quisermos. Para chamarmos colocamos.

função()

Reposta: Eu sou uma função!


def somar(x, y):#Pode colocar qualquer variável

    total = x + y
    
    print(total)

30

precisa de um parâmetro e quando chamar a função, tem q colocar as variáveis.
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Conceito de retorno.

def show():

    return 15 #retorna uma função

show()# a função contém o valor, mas para vermos precisamos printar, pois na codificação

#não foi colocado previamente o print

print(show())

# 15

#Se não usar o return, coloca o print na função.

def mult(a,b):

    return a * b
    
print(mult(10,20))

#200
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Como sugestão de prática, indicamos você a criar um novo script python seguindo as orientações a seguir:

Crie uma função que receba dois parâmetros e realize sua soma, subtração, adição e multiplicação.

Informe esses resultados através de um print ao usuário dentro da função.
 
def calculo(a,b):

    return a+b, a*b, a-b, a/b
    
print(calculo(5,10))

#(15, 50, -5, 0.5)
