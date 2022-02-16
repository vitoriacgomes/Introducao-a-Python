# :snake: Introdução a Python
Por [Vitória Gomes](https://github.com/vitoriacgomes)

* Apos configurar o ambiente baixando o Python na máquina e a IDE ( vou usar o Pycharm )

<details>
  <summary>Palavras reservadas no Python</summary>
      São elas: and, as, assert, break, class, continue, def, del, elif, else, except, exec, finally, for, from, global, if, import, in, is, lambda, not, or, pass, print, raise, return, try, while, with e yield.
</details>

## Operações Básicas no Python


       a = 10                                             
       b = 5                                                   
       soma = a + b                                          
       subtracao = a - b                                     
       multiplicacao = a * b                                 
       divisao = a / b                                       
       resto = a % b
       print (soma)                   =>     15                           
       print (subtracao)              =>     5
       print (multiplicacao)          =>     50
       print (divisao)                =>     2.0
       print (resto)                  =>     0
       
Informações: No python não é preciso apresentar as variaveis. ( print = imprimir // escrever )

#### Nomeando os resultados
       
       print ('Soma: {s}. \nSubtração: {sub}. \nMultiplicação: {m}. \nDivisão: {d}. \nResto: {r}'
       .format(s=soma, sub=subtracao, m=multiplicacao, d=divisao, r=resto))
       
       Execução:
       Soma: 15. 
       Subtração: 5. 
       Multiplicação: 50. 
       Divisão: 2.0. 
       Resto: 0
       
Informações : ***str*** = concatena o texto, ajuda o programa a indetificar o que é texto e o que é variável (È melhor usar o ***format***). ***/n*** = enter / {s} para s=soma ( ajuda a relacionar o resultador ao nome certo)

#### Interação com o usuário para operações simples

       a = int(input('Adicione o valor de A: '))
       b = int(input('Adicione o valor de B: '))
       soma = a + b
       resultado =  ('Soma: {s}'
                      .format(s=soma, sub=subtracao, m=multiplicacao, d=divisao, r=resto))
       print (resultado)
       
## Relações das variáveis 


       a = int (input('Primeiro valor:'))
       b = int (input('Segundo valor:'))
       c = int (input('Terceiro valor:'))
                                              
       if a > b and a > c:
           print ( 'O maior número é {}'.format(a))
       elif b > a and b > c:
           print('O maior númeuro é: {}'.format(b))
       else:
           print('O maior número é: {}'.format(c))
       print('Final do programa!')
       
Observações: ***if*** usado para o se, ***else*** usado para o se não e ***elif*** é a soma de if e else. // "=" (receber) e "==" (variavel resultado) // ***or*** usado como ou.
***not*** = negação a afrimação. 

## Laços de repetição
       for num in range(101):                           a = 0
       div = 0                                          while a <= 10:
       for x in range(1, num+1):          or              print(a)
          resto = num % x                               a += 1
          if resto == 0:
             div += 1
       if div == 2:
          print(num)

Observações: ***for in range*** // ***while*** usado para repetições, sequencia de numeros. ( o codigo a cima imprimi todos os numeros primos até 101 // imprimi todos os numeros ate 10)

## Listas e Operações com listas
***Imprimindo um componete de uma lista***

       lista_animal = ['gato' , 'papagaio' , 'cachorro']
       print(lista_animal[0])                                    => " gato "
       
Observações: ***[]*** esse simbolo indica a presença de listas. No caso o codigo vai imprimir "gato" pois foi a posição que eu indiquei em [0]. Ja que na sequencia o programa começa a partir de 0, se eu quisesse imprimir cachorro seria o numero 2.

***Somando uma lista***

       lista = [1, 3, 4, 5]
       print(sum(lista))        => "13"

Observações: Se eu quisesse saber o maior ou menor numero da lista era só digitar ***"max"*** ou ***"min"***

***Adicionando e Retirando itens da lista***

       lista_animal = ['gato', "cachorro", 'papagaio']
       if 'lobo' in lista_animal:
           print('Existe lobo na lista')
       else:
           print('Não existe gato na lista')
           lista_animal.append('lobo')
           print('Foi adicionado um nome componente a lista: {}'.format(lista_animal))
Dessa foram utilizando ***.append*** podemos adicionar um item não presente na lista. Mas para retirar usariamos o ***pop*** (para remover atraves da posição) e ***remove*** (atraves do nome).

***Ordenando componentes de uma lista***

         lista_animal = ['gato', "cachorro", 'papagaio', 'arara']
         lista_animal.sort()
         print(lista_animal)
Dessa forma eu consigo ordenar os componentes tanto em ordem alfabetica para letras, como numeros crescentes. Para inverter essa ordem basta usar: ***lista_animal.reverse()***

***Tuplas***
As tuplas são listas imutáveis representadas por ***'tupla = (1, 24, 38, 12)'***

Informações ***+***: ***len*** em print(len(tupla)) serve para contar os componentes tanto da tupla como da lista.

***Invertendo tuplas em lista e vice-versa***

       tupla = (3,4)                                                     lista = [1,2]  
       lista_t = list(tupla)                     or                      tupla_l = tuple(lista)
       print(type(lista_t))                                              print(type(tupla_l))
       print(lista_t)                                                    print(tupla_l)
                     
                    






