# Reinforcement learning on yubisuma

We developed a code to find the best strategy in a Japanese game called yubisuma.

This code is written in pure python.

## How to play Yubisuma

You can play with two or more people.

1. Decide who will be the first dealer by playing rock-paper-scissors or something similar.
2. All the participants form a circle and make fists with both hands as if they were handcuffed.
3. The dealer says a phrase like “Yubisuma” or “Ready, set, go” and then declares a number such as “1” or “3”.
4. The children (including the dealer) show a number by raising their thumbs or doing nothing along with the dealer’s phrase.
5. If the number shown by the children (including the dealer) matches the number declared by the dealer, the dealer can lower one of their hands.
6. If the numbers do not match, the dealer cannot lower their hand. The dealer changes clockwise or counterclockwise after each declaration.
7. The last person can't lower both of their hands loses.

## The part where I put effort

The part where the state is encoded. The state is each number of the player with i thumbs (i=0,1,2). If the thumbs raised by the players are (1, 0, 1, 0, 2), the state is (2, 2, 1). Two players with no thumbs, two players with 1 thumbs, and 1 player with two thumbs. Since the whole number of players are fixed (5), the state can be encoded to an integer from 0 to 20. This is what I did.

# License

MIT
