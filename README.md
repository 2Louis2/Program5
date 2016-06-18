//# Program5
// Day 5  of Ignatius Java Class

import javax.swing.JOptionPane;

public class Program5 {

 public static void main(String[] args) {
  // TODO Auto-generated method stub

  int money;
  String moneyOwned;
  
  moneyOwned = JOptionPane.showInputDialog("Enter an amount of dollars and cents ($30.55 would be entered as 3055): ");
  money = Integer.parseInt(moneyOwned);
  
  
  int twenty = (money / 100) / 20;
  int ten = ((money / 100) % 20) / 10;
  int five = (((money / 100) % 20) % 10) / 5;
  int one = ((((money / 100) % 20) % 10) % 5) / 1;
  
  double quarters = (((((money / 100) % 20) % 10) % 5) % 1) / 0.25;
  double dimes = ((((((money / 100) % 20) % 10) % 5) % 1) % 0.25) / 0.1;
  double nickels = (((((((money / 100) % 20) % 10) % 5) % 1) % 0.25) % 0.1) / 0.05;
  double pennies = ((((((((money /100) % 20) % 10) % 5) % 1) % 0.25) % 0.1) % 0.05) / 0.01;
   
  
  System.out.println("For money, you have: "); 
  System.out.printf("%4.2f%n", ((float)money)/100);
  
  System.out.println("");
  
  System.out.println("The number of twenty dollar bills received is " + twenty);
  System.out.println("The number of ten dollar bills received is "+ ten);
  System.out.println("The number of five dollar bills is " + five);
  System.out.println("The number of one dollar bills received is " + one);
  System.out.println("The number of quarters received as change is " + quarters);
  System.out.println("The number of dimes receieved as change is " + dimes);
  System.out.println("The number of nickels received as change is " + nickels);
  System.out.println("The number of pennies received as change is " + pennies); 
 }

}
