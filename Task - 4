Task 4 (Difficult): Intelligent DNA Pattern Search
Problem Description
A bioinformatics company needs to identify occurrences of dangerous DNA patterns inside a massive DNA sequence. Implement efficient pattern matching using KMP or Boyer-Moore algorithm.
Input Format
First line contains DNA string T.
Second line contains pattern string P.
Output Format
Print all starting indices where pattern occurs.
Constraints
1 ≤ |T| ≤ 10^6
1 ≤ |P| ≤ 10^5
Sample Input
AABAACAADAABAABA
AABA
Sample Output
0 9 12


Program:

import java.util.Scanner;

public class DNA {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        // Input DNA sequence
        System.out.print("Enter DNA Sequence: ");
        String dna = sc.nextLine().toUpperCase();

        // Input pattern to search
        System.out.print("Enter DNA Pattern: ");
        String pattern = sc.nextLine().toUpperCase();

        boolean found = false;

        System.out.println("\nPattern found at positions:");

        for (int i = 0; i <= dna.length() - pattern.length(); i++) {
            if (dna.substring(i, i + pattern.length()).equals(pattern)) {
                System.out.println((i + 1)); // 1-based position
                found = true;
            }
        }

        if (!found) {
            System.out.println("Pattern not found.");
        }

        sc.close();
    }
}
