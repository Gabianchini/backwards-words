# backwards-words
  Foi criado um script que visa inverter as palavras escolhidas pelo usuário.
  É Possível acessar caracteres escolhidos de uma string em Python usando a notação []. Neste método de ordem de caracteres de uma string, o primeiro caracter consta como índice 0, o segundo índice 1, e assim por diante, conforme ilustrado no exemplo abaixo.

s = "julia"
print(s[0])
print(s[2])
'j'
'l'

  No caso da string "julia", temos a seguinte associação entre índices e dígitos:

j u l i a 
0 1 2 3 4 

  Podemos também acessar os elementos em ordem reversa usando índices negativos. Neste sistema, o último caracter de uma string consta como índice −1, o penúltimo no índice −2, e assim por diante, como mostrado no exemplo abaixo.

s = "julia!"
print(s[-1])
print(s[-2])
print(s[-3])
'a'
'i'
'l'
 
  Para efetuar a inversão de palavras é necessário também "fatiar" uma string.Ou seja, uma fatia de uma string, logo,uma substring, pode ser acessada se fornecermos os índices do começo e do final da fatia que desejamos analisar, como mostrado abaixo:

s[1:3]
'ul'

  Além disso, perceba que o índice do final da fatia não é incluído nela. No exemplo acima, o [1:3] nos retornou dois caracteres e não três. Foram retornados o caracter no índice 1 e o caracter no índice 2, mas não o caracter no índice 3.

  É possível ainda especificar um parâmetro que indica quantos caracteres devem ser processados de cada vez. Por exemplo, se quisermos imprimir somente os caracteres nos índices pares ou ímpares de uma string, podemos fazer assim:

  Um outro exemplo útil do uso da técnica de slicing para manipulação de strings é inverter uma palavra ou frase usando somente operações de slicing:

frase = "Mundo mundo vasto mundo"
print(frase[::-1])
odnum otsav odnum odnuM

  No exemplo acima, usamos um terceiro parâmetro do recurso de slicing para indicar que retornamos toda a frase (os ::) e logo em seguida dizemos que faremos isso de trás para frente (por meio do −1 no final). Mais especificamente, o −1 indica que estamos saltando um caracter de cada vez, começando de trás para frente (o que é feito por meio do sinal de menos).
 Então, para resumir, a sintaxe de slicing de strings é a seguinte [início:fim:salto], onde:

início é o primeiro índice a ser considerado (o primeiro caracter da string é considerado caso este valor seja omitido);

fim - 1 é o último índice a ser considerado (o último caracter da string é considerado caso este valor seja omitido); e

salto indica quantos caracteres devem ser saltados em cada etapa (o valor 1 é considerado por padrão, e um sinal de menos deve ser usado para percorrer a string em ordem reversa).
