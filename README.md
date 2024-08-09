# 3C-HELOISE
# Mini Jogo de Reciclagem

Este é um mini jogo de reciclagem simples em Python. O objetivo do jogo é escolher o tipo correto de lixo para reciclagem.
# jogo_reciclagem.py

import random

def jogo():
    lixo = ['papel', 'vidro', 'plástico', 'metal']
    correto = random.choice(lixo)
    
    print("Bem-vindo ao Jogo de Reciclagem!")
    print("Você precisa escolher o tipo correto de lixo para reciclagem.")
    print("Tipos de lixo disponíveis: papel, vidro, plástico, metal")
    
    escolha = input("Escolha um tipo de lixo: ").strip().lower()
    
    if escolha == correto:
        print("Correto! Você reciclou o lixo corretamente.")
    else:
        print(f"Incorreto. O tipo correto de lixo era: {correto}")

if __name__ == "__main__":
    jogo()
# Mini Jogo de Reciclagem

Este é um mini jogo de reciclagem simples em Python. O objetivo do jogo é escolher o tipo correto de lixo para reciclagem.

## Como Jogar

1. Execute o jogo com o comando `python jogo_reciclagem.py`.
2. Escolha um tipo de lixo quando solicitado.
3. O jogo informará se a escolha está correta ou não.

## Requisitos

- Python 3.x
python jogo_reciclagem.py
# test_jogo_reciclagem.py

import unittest
from jogo_reciclagem import jogo
class TestJogoReciclagem(unittest.TestCase):
    def test_jogo(self):
    self.assertEqual(jogo('papel'), 'Correto! Você reciclou o lixo corretamente.')
    if __name__ == '__main__':
    unittest.main()
    python -m unittest test_jogo_reciclagem.py
python -m unittest test_jogo_reciclagem.py
