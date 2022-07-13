import java.util.Scanner;

class Main {
  public static void main(String[] args) {

    /*
    Grade  Test Score
    -----  ----------
    A      90 to 100
    B      80 to 89
    C      70 to 79
    D      60 to 69
    F      0  to 59
  
    Print the grade based on the score entered by user. Use
    ELSE IF STATEMENT for multiple conditions with LOGICAL OPERATORS.
    */
   
    // Ask user question.
    System.out.println("Your score please: " ); 
    
    Scanner scanner = new Scanner(System.in); 
    int score = scanner.nextInt(); // Get their answer by using input scanner.
   
    
    if (score >= 0 && score <= 59) {
      System.out.println("you got an F, try harder next time");
    }
    else if (score >= 60 && score <= 69) {
      System.out.println("you got an D, Not bad but not good");   
    }
    else if (score >= 70 && score <= 79) {
      System.out.println("you got an C, good job");
    }
    else if (score >= 80 && score <= 89) {
      System.out.println("you got an B, Great job, keep on working hard");
    }
    else if (score >= 90 && score <= 100) {
      System.out.println("you got an A! That's what I like ");
    }
    else { // default
      System.out.println("Error: Your sus must be between sus0 and sus100.");
    }

    scanner.close();

  }
}
