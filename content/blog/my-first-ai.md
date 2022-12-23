---
title: "My First AI: Black Jack Machine Learning"
date: 2022-12-22T20:30:41-06:00
draft: false 
---

I wrote my first artificial intelligence program in Java. The computer scientists reading this most likely sighed and for all you non-computer scientists out there let me explain why.

Imagine trying to make modern dance music with a piano. A piano’s great but not for modern dance music. This is what using Java for AI is like. It’s possible but the result is not pretty, but Java was all I knew.

That all being said, my first AI program wasn’t bad. I wrote it way back in my sophomore year of high school, late 2017, but I still remember the ins and outs of it. It was a machine-learning algorithm that would learn to play blackjack.

First I had to code the game itself. To do this I created arrays for the deck, the hands of my machine and the dealer. Then I created the basic game of blackjack where the player and dealer are dealt two cards and the player decides to hit or stay, and the winner is the one closest to 21 without going over.

A few side notes and limitations. First, I chose to play house wins on the tie. Second, the player, my machine, can’t see the dealer’s cards. This aspect is unrealistic but simplifies the game to make it much easier to “teach” the computer.

Moving to the learning aspect of the program. The machine learning in this program revolved around one decision一hit or stay. Machine learning is, in essence, using data to decide what decision is best given the circumstances: this is the learning that machines do, basically, the machine just creates a function from a lot of experience.

How would the computer do this though? There are many ways of teaching a computer; however, I settled on reinforcement learning. Reinforcement learning is very similar to how a dog is trained. If the dog does something good, let’s say they sit when told, they get a treat. The treat reinforces good behavior and the dog is now more likely to sit when told.

So, the computer starts “untrained” and at every possible number of points (four to twenty, because the computer is dealt two cards that at least could be two twos and because a twenty one would result in a win) the computer has a fifty-fifty chance of hitting or not.

With every game played the computer tweaks the odds based on if they won or not. If the computer won it would want to repeat what it did so it would increase the chances of hitting where it hit: the opposite happens for when it loses.

So after one million games what has the computer learned? On average, the computer won 113% more games at the end than the beginning. Could you do better just by creating an algorithm using statistics of winning? Of course, but that is not as fun as seeing how a computer reacts to a machine learning algorithm.

The computer learned to always hit on 11 and never on 20 which makes sense, but on earlier numbers the hitting percentage actually decreases. This is most likely due to how the algorithm is written. If the computer gets 4 on the draw then at the end busts it will decrease hitting on 4.

If I were to rewrite this algorithm I would build in a way to get around this; however, there is no simple way to do so. Perhaps the older the hit the less it is tweaked, but this also introduces other problems.

In conclusion, this algorithm was very fun to write and interesting to see what the computer learned.
