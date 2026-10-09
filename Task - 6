Task 6 (Difficult): Ride Sharing Platform Simulator
Problem Description
Design an object-oriented ride sharing system with reusable classes for Driver, Rider, Vehicle, and Trip. Support polymorphic fare calculation for Bike, Auto, and Cab rides. Include exception handling for invalid bookings.
Input Format
First line contains integer N.
Next N lines contain ride type and distance.
Output Format
Display fare for each trip.
Constraints
1 ≤ N ≤ 10^5
Sample Input
3
Bike 10
Cab 15
Auto 8
Sample Output
50
180
96

    program:


import java.util.Scanner;

public class Ride {

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        String customerName = "";
        String pickup = "";
        String destination = "";
        double distance = 0;
        double fare = 0;

        int choice;

        do {
            System.out.println("\n===== Ride Sharing Platform Simulator =====");
            System.out.println("1. Book Ride");
            System.out.println("2. View Ride Details");
            System.out.println("3. Exit");
            System.out.print("Enter your choice: ");

            choice = sc.nextInt();
            sc.nextLine(); // Consume newline

            switch (choice) {

                case 1:
                    System.out.print("Enter Customer Name: ");
                    customerName = sc.nextLine();

                    System.out.print("Enter Pickup Location: ");
                    pickup = sc.nextLine();

                    System.out.print("Enter Destination: ");
                    destination = sc.nextLine();

                    System.out.print("Enter Distance (km): ");
                    distance = sc.nextDouble();

                    fare = 50 + (distance * 12); // Base fare + per km charge

                    System.out.println("\nRide Booked Successfully!");
                    System.out.println("Estimated Fare: ₹" + fare);
                    break;

                case 2:
                    if (customerName.equals("")) {
                        System.out.println("No ride booked yet.");
                    } else {
                        System.out.println("\n----- Ride Details -----");
                        System.out.println("Customer Name : " + customerName);
                        System.out.println("Pickup        : " + pickup);
                        System.out.println("Destination   : " + destination);
                        System.out.println("Distance      : " + distance + " km");
                        System.out.println("Estimated Fare: ₹" + fare);
                    }
                    break;

                case 3:
                    System.out.println("Thank you for using the Ride Sharing Platform!");
                    break;

                default:
                    System.out.println("Invalid choice. Please try again.");
            }

        } while (choice != 3);

        sc.close();
    }
}
