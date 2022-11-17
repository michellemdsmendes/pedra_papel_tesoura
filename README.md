from random import randint
from time import sleep
itens = ('pedra', 'papel', 'tesoura')
computador = randint(0, 2)
print('''SUAS OPÇÕES:
[ 0 ] PEDRA
[ 1 ] PAPEL
[ 2 ] TESOURA''')
jogador = int(input('QUAL É A SUA JOGADA? '))
print('-=' * 11)
sleep(1)
print('JO')
sleep(1)
print('KEN')
sleep(1)
print('PO!!')
print('-=' * 11)
print('Computador jogou {}'.format(itens[computador]))
print('Jogador jogou {}'.format(itens[jogador]))
if computador == 0:  # computador jogou PEDRA
  if jogador == 0:
    print('EMPATE')
  elif jogador == 1:
    print('JOGADOR VENCE')
  elif jogador == 2:
    print('COMPUTADOR VENCE')
  else:
    print('JOGADA INVÁLIDA!')
elif computador == 1:  # computador jogou PAPEL
  if jogador == 0:
    print('COMPUTADOR VENCE')
  elif jogador == 1:
    print('EMPATE')
  elif jogador == 2:
    print('JOGADOR VENCE')
  else:
    print('JOGADA INVÁLIDA!')
elif computador == 2:  # computador jogou TESOURA
  if jogador == 0:
    print('JOGADOR VENCE')
  elif jogador == 1:
    print('COMPUTADOR VENCE')
  elif jogador == 2:
    print('EMPATE')
  else:
    print('JOGADA INVÁLIDA!')
