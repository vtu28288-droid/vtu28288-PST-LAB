Task 3 (Easy): Maximum Profit Analyzer
Problem Description
Given daily profit/loss values, find the maximum possible profit obtainable from a contiguous sequence of days using Kadane’s Algorithm.
Input Format
First line contains integer N.
Second line contains N integers.
Output Format
Print maximum subarray sum.
Constraints
1 ≤ N ≤ 10^5
Sample Input
8
-2 -3 4 -1 -2 1 5 -3
Sample Output
7

    program:


import java.util.Scanner;

public class Max {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter number of days: ");
        int n = sc.nextInt();

        int[] prices = new int[n];

        System.out.println("Enter stock prices:");
        for (int i = 0; i < n; i++) {
            prices[i] = sc.nextInt();
        }

        int minPrice = prices[0];
        int maxProfit = 0;
        int buyPrice = prices[0];
        int sellPrice = prices[0];

        for (int i = 1; i < n; i++) {
            if (prices[i] < minPrice) {
                minPrice = prices[i];
            }

            if (prices[i] - minPrice > maxProfit) {
                maxProfit = prices[i] - minPrice;
                buyPrice = minPrice;
                sellPrice = prices[i];
            }
        }

        System.out.println("Buy Price : " + buyPrice);
        System.out.println("Sell Price: " + sellPrice);
        System.out.println("Maximum Profit: " + maxProfit);

        sc.close();
    }
}
