# Exercicio058.py

from random import randint
comp = randint(0, 10)
print('Sou seu pior pesadelo, consegue advinhar em quee numero pensei de 0 a 10?')
acertou = False
palpites = 0
while not acertou:
    jogador = int(input('Qual seu palpite? '))
    palpites += 1
    if jogador == comp:
        acertou = True
    else:
        if jogador < comp:
            print('Mais...Tente mais uma vez')
        elif jogador > comp:
            print('Menos...Tente mais uma vez')
print('Acertoou com {} tentativas'.format(palpites))
