# Lista-3---Linguagem-de-programacao
Exercícios do 1 ao 8 em python
===================================================================================================
1) Escreva um programa que leia uma matriz de ordem 3 x 5 de elementos inteiros,
  calcule e mostre na tela:
  a) menor número da matriz;
  b) soma dos números múltiplos de 3 da matriz;
  c) maior número da 3ª coluna da matriz (índice 2);
  d) média dos números da matriz;


from random import randint
matriz=[]
for i in range(3):
    linha=[]
    for j in range(5):
        linha.append(randint(1,99))
    matriz.append(linha)
menor=matriz[0][0]
for i in range(3):
    print(matriz[i])
soma=0
for i in range(3):
    soma=sum(matriz[i])
media=soma/15
soma2=0
for linha in matriz:
    for valor in linha:
        if valor%3==0:
            soma2+=valor
        if valor<menor:
            menor=valor
maior=matriz[2][0]
for valor in matriz[2]:
    if valor>maior:
        maior=valor

print(f'O menor número da matriz é {menor}')
print(f'A soma dos números múltiplos de 3 da matriz resulta em {soma2}')
print(f'A média dos números da matriz resulta em {media}')
print(f'O maior número da 3ª coluna da matriz é {maior}')
===================================================================================================
2) Escreva um programa que preencha uma matriz 4 x 6 com números inteiros,
  calcule e mostre na tela:
  a) A quantidade de números que estão no intervalo entre 10 e 30
  b) A soma dos números maiores que 10 e pares
  c) A soma dos números que estão na quarta coluna da matriz
  d) A média dos números da matriz que estão na terceira linha

from random import randint
matriz=[]
for i in range(4):
    linha=[]
    for j in range(6):
        linha.append(randint(1,99))
    matriz.append(linha)
for i in range(4):
    print(matriz[i])
cont=soma=0
for linha in matriz:
    for valor in linha:
        if valor>10 and valor<30:
            cont+=1
        if valor%2==0 and valor>10:
            soma+=valor
soma2=0
for valor in matriz[3]:
    soma2+=valor
soma3=0
for valor in matriz[2]:
    soma3=sum(matriz[2])
media=soma3/6
print(f'A quantidade de números que estão no intervalo entre 10 e 30 é igual a {cont}')
print(f'A soma dos números maiores que 10 e pares resulta em {soma}')
print(f'A soma dos números que estão na quarta coluna da matriz resulta em {soma2}')
print(f'A média dos números da matriz que estão na terceira linha é igual a {media}')
===================================================================================================
5) Escreva um programa que preencha uma matriz 4 x 3 com números inteiros,
  calcule e mostre na tela:
  a) A soma dos elementos que estão na 2ª e 4ª linha da matriz
  b) A soma dos números primos

from random import randint
matriz=[]
for i in range(4):
    linha=[]
    for j in range(3):
        linha.append(randint(1,99))
    matriz.append(linha)
for i in range(4):
    print(matriz[i])
    
soma=0
for valor in matriz[1]:
    soma+=valor
print(f'Resultado da soma da 2ª linha da matriz: {soma}')

soma2=0
for valor in matriz[3]:
    soma2+=valor
print(f'Resultado da soma da 4ª linha da matriz: {soma2}')
total=soma+soma2
print(f'A soma dos elementos que estão na 2ª e 4ª linha da matriz resulta em {total}'
===================================================================================================
===================================================================================================
