# Addition Game
## Introduction
This assignment deals with how to create a four round addition game that increases in difficulty with every correct answer and decreases with incorrect answers. 
## Outline
``` java
/* Generate a random numbers 
* Prompt the user to add them together
* If correct add points and increase the difficulty
* When incorrect do not add points and decrease difficulty
* After four rounds display score
*/
```
## References and Literature
/* Liang Java 10th Edition Pg. 77
* Google searches 
* Dr. Evert, Instructor Irvin, and class mates
*/

## Code
(This is based on the code written by Dr. Evert since I did not get the code correct)
``` java
import java.util.Scanner;
public class MathGame {
	public static void main(String[] args) {
		
	System.out.println("Hello Class!");

		int score = 0;
		int hardness = 10;
		 		
		// Round 1
		// Generate 2 random numbers
		int number1 = (int)(Math.random() * hardness);
		int number2 = (int)(Math.random() * hardness);
		int correctAnswer = number1 + number2;
		 		
		//  Ask the user to add these two numbers together
				
		System.out.println("What integer is " + number1 + " + " + number2 + "?");
		System.out.println("Please enter integers only.");
		
		 // Read in their response
		 Scanner input = new Scanner(System.in);
		 int studentAnswer = input.nextInt();
		 // Check if the answer was correct
		
		 // IF correct
		if (studentAnswer == correctAnswer){
		if(studentAnswer == correctAnswer){
		//IF correct
		 //Tell them it was correct
		System.out.println("Your answer was correct.");
		// Give them points
		score += hardness;
		System.out.println("Your score is now: " + score);
		// Make the next question harder
		System.out.println("Answer was correct");
				}
		// IF not correct
		else{
		hardness *= 10;
		System.out.println("The next hardness will be: " + hardness);
		} }else{
		// IF not correct
		// Tell them it was wrong
		System.out.println("Answer was not correct");
		System.out.println("Your answer was not correct.");
		// Tell them the correct answer
		System.out.println("The correct answer was: " + correctAnswer);
		// Do not give them points
		score += 0;
		// Make the next question easier
		if (hardness > 10){
		hardness /= 10;
		System.out.println("Your hardness is now: " + hardness);
		}else{
		System.out.println("Your hardness is at the lowest level");
		System.out.println("Your hardness is now: " + hardness);
					}
					
					
		 		}
		
		System.out.println("End of round 1.");
				
		 // Round 2
		number1 = (int)(Math.random() * hardness);
		number2 = (int)(Math.random() * hardness);
		correctAnswer = number1 + number2;
				
		 //  Ask the user to add these two numbers together
		System.out.println("What integer is " + number1 + " + " + number2 + "?");
		System.out.println("Please enter integers only.");
		//  Read in their response
		studentAnswer = input.nextInt();
		 
		if(studentAnswer == correctAnswer){
		// IF correct
		// Tell them it was correct
		System.out.println("Your answer was correct.");
		score += hardness;
		System.out.println("Your score is now: " + score);
		// Make the next question harder
		hardness *= 10;
		System.out.println("The next hardness will be: " + hardness);
		}else{
		// IF not correct
		// Tell them it was wrong
		System.out.println("Your answer was not correct.")					
		// Tell them the correct answer
		System.out.println("The correct answer was: " + correctAnswer);			
		// Do not give them points
		score += 0;
		// Make the next question easier
		if (hardness > 10){
		hardness /= 10;
		System.out.println("Your hardness is now: " + hardness);
		}else{
		System.out.println("Your hardness is at the lowest level");
		System.out.println("Your hardness is now: " + hardness);
					}
					
					
				}
		
		System.out.println("End of round 2.");
				
		// Round 3
		// Generate 2 random numbers
		number1 = (int)(Math.random() * hardness);
		number2 = (int)(Math.random() * hardness);
		correctAnswer = number1 + number2;
				
		//  Ask the user to add these two numbers together
		System.out.println("What integer is " + number1 + " + " + number2 + "?");
		System.out.println("Please enter integers only.");
		//  Read in their response
		studentAnswer = input.nextInt();
		 
		if(studentAnswer == correctAnswer){
		// IF correct
		// Tell them it was correct
		System.out.println("Your answer was correct.");
		// Give them points
		score += hardness;
		System.out.println("Your score is now: " + score);
		// Make the next question harder
		hardness *= 10;
		System.out.println("The next hardness will be: " + hardness);
		}else{
		// IF not correct
		// Tell them it was wrong
		System.out.println("Your answer was not correct.");
		// Tell them the correct answer
		System.out.println("The correct answer was: " + correctAnswer);
		// Do not give them points
		score += 0;
		// Make the next question easier
		if (hardness > 10){
		hardness /= 10;
		System.out.println("Your hardness is now: " + hardness);
		}else{
		System.out.println("Your hardness is at the lowest level");
		System.out.println("Your hardness is now: " + hardness);
					}
					
					
				}
		
		System.out.println("End of round 3.");
		// Round 4
		//	Generate 2 random numbers
		number1 = (int)(Math.random() * hardness);						
		number2 = (int)(Math.random() * hardness);
		correctAnswer = number1 + number2;
				
		//  Ask the user to add these two numbers together
		System.out.println("Please enter integers only.");
		//  Read in their response
		studentAnswer = input.nextInt();
		 	
		if(studentAnswer == correctAnswer){
		// IF correct
		// Tell them it was correct
		System.out.println("Your answer was correct.");
		// Give them points
		score += hardness;
		System.out.println("Your score is now: " + score);
		// Make the next question harder
		hardness *= 10;
		System.out.println("The next hardness will be: " + hardness);
		}else{
		// IF not correct
		// Tell them it was wrong
		System.out.println("Your answer was not correct.");
		// Tell them the correct answer
		System.out.println("The correct answer was: " + correctAnswer);
		// Do not give them points
		score += 0;
		// Make the next question easier
		if (hardness > 10){
		hardness /= 10;
		System.out.println("Your hardness is now: " + hardness);
		}else{
		System.out.println("Your hardness is at the lowest level");
		System.out.println("Your hardness is now: " + hardness);
					}
					
					
				}
		
		System.out.println("End of round 4.");
		System.out.println("Your final score is: " + score);
		 
		 	}
}

```
## Console Output
Hello Class!
What integer is 5 + 3?
Please enter integers only.
8
Your answer was correct.
Your score is now: 10
Answer was correct
End of round 1.
What integer is 3 + 3?
Please enter integers only.
6
Your answer was correct.
Your score is now: 20
The next hardness will be: 100
End of round 2.
What integer is 91 + 36?
Please enter integers only.
127
Your answer was correct.
Your score is now: 120
The next hardness will be: 1000
End of round 3.
What integer is 957 + 969?
Please enter integers only.
1926
Your answer was correct.
Your score is now: 1120
The next hardness will be: 10000
End of round 4.
Your final score is: 1120

## Summary
This assignment was to create an addition game that progressively got more difficult with each correct answer.
While originally I didn’t get all of the code right but I used the code posted by Dr. Evert on git hub to complete it.
This code works by using if else statements to give the player the proper difficulty based on their performance and after 
four rounds it displays the score achieved. This assignment helped me further my knowledge with if and else statements and 
wonder what other ways there are to do this simpler. 
