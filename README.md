# **_WAR_** 

Here's the popular card game, War.
Each player draws a card from the deck and the player with the highest card wins.
Built war by defining classes, representing a card, a deck, a player and finally, the game itself.
---

- A class, then models playing cards. *__Suits and values__* are class variables. Suits is a list of strings representing all the suits in a deck of cards.
Values is a list of strings representing all the numbers in a deck of cards. The values list has none at index 0 and 1 so that the numbers in the list match their index.
Card objects have two instance variables suit and value together.The integers stored in these instance variables represent what kind of card the card object is.
For example, if we create a two of hearts by making a new card object and passing it the numbers two and one as parameters.

- *__lt and gt are magic methods__*, so we can use them to compare to card objects in an expression using the greater than and less than operators.
In this example, Python calls the magic method lt on the card one object and passes in card two as a parameter.
If the first card's value is higher than the second, the method returns true.If the second card's value is higher, the method returns false.
If the two cards are equal, the method returns whatever card has the highest suit.This works because the suits are in order from least powerful to most powerful. The lt magic method works the same way, only it checks to see if card one is less than card two.

The magic method uses the value and suit instance variables to look up the value and suit of a card in the values and suits lists.
and returns them so you can print the card.

- Now there's a class, to represent a *__deck of cards__*. When initialize the deck object, this code creates card objects representing all of the cards in
the 52 card deck and depends them to the cards list.The loop is from 2 to 14 because the deck starts at two and ends at ace, which is card 14.
Each time around the inner loop, Python creates a new card using the integer from the outer loop as the value and the integer from the inner loop as the suit.

The *__shuffle__* method from the random module randomly rearranges the items in the cards list, mimicking the shuffling of a deck of cards.
Our deck has one other method that removes and returns a card from the cards list or returns none if it is empty.

- Now creating a class to represent each player in the game to keep track of their cards and how many rounds they've won.
*__The player class__* has three instance variables, winds to keep track of how many rounds a player has one card to represent the card a player is currently holding and a name to keep track of a player's name.



- Finally,a class to represent the game.
When created the *__game object__*, Python calls the init method and you use the input function to collect the names of the players in the game and save them an instance variables.
Next,to create a new deck object and two player objects, which also stores an instance variables.
The method wins prints the name of whatever player won that round.
The method draw takes the name and card of each player and prints the card they drew.
This method starts the game.The while loop in it continues if there are more than two cards in the deck, if player one ever enters the queue during their turn,the line of code ends the game.
---




 Each time through the loop, your code draws two cards and assigns one to each player.

Next,to print the name of each player and the card they drew. Compare the two cards to see which card is greater.
And increment the wins instance variable of the player with the greater card.
When the deck object runs out of cards, the loop inside of play game ends and you use the winner method to determine who won the game.

Finally, it prints a message that says the war is over and the name of the player that won.
Here is your full game.

