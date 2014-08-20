---
title: Hearthstone Cockatrice Port
description: Assets for playing hearthstone using the Cockatrice application
layout: default
---

# Setting up

1. Download and install Cockatrice from [Woogerworks](http://woogerworks.com/).
1. Clone this repository to a folder of your choosing.
1. Open the Cockatrice settings. The following paths are relative to the folder
   containing the cloned repo.
  - Change the picture directory to point to the /pics folder.
  - Change the card database path to /db/cards.xml, and the token database path
    to /db/tokens.xml
  - Optionally, change the card back to /card_back.jpg
1. Connect to the woogerworks server to play. (Note that Cockatrice is intended
   for playing Magic: the Gathering. Arrange games with friends through other
   means of communication.)

Instead of cloning the repository you can always choose to just download the
repository as a zip. However, cloning the repository lets you retrive any
updates easily.

It might be the case that you use Cockatrice to play Magic as well. In that
situation application virtualization could be the solution. There are multiple
options to choose from, but one suggestion (for windows) would be
[Sandboxie](http://www.sandboxie.com/). Instructions for setting up application
virtualization is outside the scope of this readme.    

## Additional assets

A basic deck template for each class is provided under the /deck_templates
folder. These templates are preset with a sideboard containing the hero card
and any hero specific cards.  

# Screenshots

Hunter secret deck on the right track:

![screenshot1](images/Screenshot1.jpg)

A krushing phrase:

![screenshot2](images/Screenshot2.jpg)

# Best practices

Cockatrice is intended for playing Magic: the Gathering, but with some
adoptions it can house sessions of Hearthstone play.

- The sideboard (shown with Ctrl+F3) is used to hold the hero card, hero
  specific cards, a Mana Crystal and The Coin, as well as any token cards for
  the deck.
- If you create token through the token dialog, always uncheck the destroy
  token checkbox since the cards may need to be picked up to your hand. Note that
  cloning cards (with Ctrl+J) always creates tokens that are destroyed when
  leaving the playing field.
- Use the Mana Crystal from the sideboard (and clones thereof) to track your
  mana. Tap the crystals to mark how much mana you have used that turn.
  - When playing as Shaman, move crystals further apart to mark overloaded mana
    and tap them, starting with the rightmost crystal, to mark overloaded mana
	on a turn when you have mana already locked.
- Mark the current hp of minions with red counters. Always track the current hp
  rather than damage taken.
- Track armor with yellow counters on the hero card.
- When using the die to randomly choose a character and/or minion assign
  numbers in this order (for those applicable). The first number is your
  opponent, then the opponent's minions, your own minions, and last yourself as
  the last number.
- To perform "random card from deck" effects, use the View library feature,
  count the number of creatures and roll a die.  
- To perform "random card from opponent's deck" effects, use the "Show library
  to other player" feature. The opponent then creates a token of two cards.
- Playing or moving a card secretly, e.g. when playing Secret cards, can be
  done by dragging the card while holding down shift. This places the card face
  down. You can peak at the card by selecting "Peak at card face" in the card's
  context menu (then press the card in the chat to see the card picture).

# Credits

Credit goes to phantasma0000 which made the initial port, published at
[Hearthstone Port Project](http://hearthstoneport.wordpress.com/), on which my
port is a continuation.

Further thanks to [Hearthhead](http://hearthhead.com/) which I have used as my
card picture source.

Special thanks to Esk4 which made original art to represent the custom mana
crystal card.

# Legal

This work is in the Public Domain so as to not infringe on any copyright.

I also concur with the disclamer phantasma0000 uses at
[Hearthstone Port](http://hearthstoneport.wordpress.com/):

> This port is designed solely for use of non-commercial testing of decks and
gameplay and acts as a virtual solution for those who do not want to print out
cards (which has been allowed by Blizzard). This project is not affiliated with
Blizzard Entertainment in any way.  The point of this project is not to copy or
distribute Blizzard Entertainment materials and will be brought down
immediately upon request.
