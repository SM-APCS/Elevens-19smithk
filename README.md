# Elevens Lab

1. Explain in your own words the relationship between a deck and a card.

A deck is made up of a bunch of cards. The deck is an arraylist of cards.

2. Consider the deck initialized with the statements below. How many cards does the deck contain?

String[] ranks = {"jack", "queen", "king"};
String[] suits = {"blue", "red"};
int[] pointValues = {11, 12, 13};
Deck d = new Deck(ranks, suits, pointValues);

The code errored; 'index out of bounds'. The array "suits" doesn't have as many values as the other two arrays.


3. The game of Twenty-One is played with a deck of 52 cards. Ranks run from ace (highest) down to 2 (lowest). Suits are spades, hearts, diamonds, and clubs as in many other games. A face card has point value 10; an ace has point value 11; point values for 2, �c, 10 are 2, �c, 10, respectively. Specify the contents of the ranks, suits, and pointValues arrays so that the statement initializes a deck for a Twenty-One game.

Deck d = new Deck(ranks, suits, pointValues);  

You would need the ranks array for "King" " Ace" "Queen" kinda stuff to set the english names to cards 11-13. Then you would have the suits array with the different suits repeated 13 times for each group of 13 cards. The the pointlessValues would have 2-13 repeated 3 times. 

4. Does the order of elements of the ranks, suits, and pointValues arrays matter?

Yes because the ranks suits and pointValues create the cards that make up the deck. 


ACTIVITY 3 

This is the Flip class for question 2:

public class...

public class Activity3Methods {

	public static void main(String[] args)
  {
		
		int[] firstArray = {1,2,5,0,3};
		int[] secondArray = {2,3,5,1,0};
		System.out.println(arePermutations(firstArray,secondArray));
		/*System.out.println(flip());
		System.out.println(flip());
		System.out.println(flip());
		System.out.println(flip());*/
	}
	
	public static String flip(){
		int random = (int) (Math.random()*(2));
		
		if(random == 1 || random == 2)
    {
			return "heads";
		}
		else
    {
			return "tails";
		}
		
	}
	
	
	public static boolean arePermutations(int[] one, int[]two)
  {
		int i = 0;
		boolean returnThis = true;
		while(i < one.length)
    {
			
			int numbInOne = one[i];
			if(arrayContains(numbInOne,two))
      {
				
			}
			else
      {
				returnThis = false;
				break;
			}
			i++;
		}
		
		return returnThis;
	}
	
	public static boolean arrayContains(int number, int[] intArray){
		int matches = 0;
		for (int k = 0; k < intArray.length; k++)
    {
			if(number == intArray[k]
    ){
				matches++;
			}
		}
		
		if(matches > 0){
			return true;
		}
		else{
			return false;
		}
	}
	
}

3. Suppose that the initial contents of the values array in Shuffler.java are {1, 2, 3, 4}. For what sequence of random integers would the efficient selection shuffle change values to contain {4, 3, 2, 1}?
The random sequence would be 3,2,1,0


Activity 6 

1. List all possible plays for the board 5♠ 4♥ 2♦ 6♣ A♠ J♥ K♦ 5♣ 2♠

The possible plays are 5♠ and 6♣, 6♣ and 5♣.

2. If the deck is empty and the board has three cards left, must they be J, Q, and K? Why or why not?

Yes, there are only a certain amount of pairs to be made. You have to have a pair left. 

3. Does the game involve any strategy? That is, when more than one play is possible, does it matter which one is chosen? Briefly explain your answer.

The game is mainly based on a high level of luck, but there is also a little bit of strategy. If you pick the triple thing, you get theree new cards. This helps with the pairs. :) 








