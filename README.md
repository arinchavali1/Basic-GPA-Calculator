# Basic-GPA-Calculator

import java.util.Scanner;
public class MyClass {
    public static void main(String args[]) {
      Scanner scan = new Scanner(System.in);
      System.out.println("How many classes are you enrolled in? ");
      double classno = scan.nextInt();
      double count = 0;
      double gpa = 0;

      
      for(int i = 0; i<classno; i++)
      {

          System.out.println("Enter your grade: ");
          int grade = scan.nextInt();

          
          if (grade >=90 && grade <=100)
          {
              gpa = 4;
              count +=gpa;
          }
          
          else if (grade >=80 && grade <=89)
          {
              gpa = 3;
              count+=gpa;
          }
          
          else if(grade >=70 && grade <= 79)
          {
              gpa = 2;
              count+=gpa;
          }
          
         else if (grade >=60 && grade <=69)
          {
              gpa = 2;
              count+=gpa;
          }
          else if (grade <=59)
          {
             gpa = 0;
             count+=gpa;
          }
          else
            System.out.println("Enter a valid numerical grade value please.");
            
        
         
      }
      
      double averagegpa = count/classno;
      System.out.println("Your GPA is: " + averagegpa);
      
      
      
     
    }
}
