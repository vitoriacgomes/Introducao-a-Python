# Introdução a Python
Por [Vitória Gomes](https://github.com/vitoriacgomes)

* Apos configurar o ambiente baixando o Python na máquina e a IDE ( vou usar o Pycharm )

### Operações Básicas no Python


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
