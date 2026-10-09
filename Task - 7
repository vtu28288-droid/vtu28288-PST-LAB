Task 7 (Easy): Hashtag Frequency Counter
Problem Description
Count frequency of hashtags appearing in social media posts using maps/dictionaries.
Input Format
First line contains integer N.
Next N lines contain hashtags.
Output Format
Display hashtag frequencies.
Sample Input
5
java
python
java
ai
python
Sample Output
java 2
python 2
ai 1

    
Program:

import java.util.*;

public class HashtagFrequency {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter no of hashtags: ");
        int n = sc.nextInt();
        sc.nextLine();

        HashMap<String, Integer> map = new LinkedHashMap<>();

        System.out.println("Enter hashtags:");

        for (int i = 0; i < n; i++) {
            String hashtag = sc.nextLine().trim().toLowerCase();
            map.put(hashtag, map.getOrDefault(hashtag, 0) + 1);
        }

        for (Map.Entry<String, Integer> entry : map.entrySet()) {
            System.out.println(entry.getKey() + " " + entry.getValue());
        }

        sc.close();
    }
}
