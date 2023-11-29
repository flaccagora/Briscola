# BRISCOLA

## Description
This is a simple implementation of the card game Briscola. The game is played between two players, one of which is the computer. The game is played with a deck of 40 cards, and the goal is to score more points than the opponent. The game is played in turns, and each turn consists of two phases: the first player plays a card, then the second player plays a card. The winner of the turn is the player who played the highest card, according to the following order: ace, three, king, queen, jack, seven, six, five, four, two.The game ends when all the cards have been played. The player with the highest score wins the game.

## How to run

Before running, install torch
> pip install torch torchvision torchaudio


then install rlcard:

> pip install .

### Train

Usually something like this:

> python3 ./examples/run_rl_finale.py --log_dir="experiments/briscola_dqn_final/"


### Play against Agent

Default play against dqn agent, change code if you want to play against nfsp agent or different checkpoint.

> python3 ./examples/human/briscola_human.py --opp_hand_visible="True"

### Test
Per testare con diversi reward sostituire i file in `Different_Rewards` con quelli in `rlcard/env/Briscola`  e `rlcard/utils` e lanciare il comando `pip install .` da terminale.
