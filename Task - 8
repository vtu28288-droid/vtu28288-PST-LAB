Task 8 (Difficult): Smart Traffic Navigation System
Problem Description
A smart city application stores road connectivity information using nested collections. Given city junctions and roads, determine whether a route exists between two junctions using graph representation with collections.
Input Format
First line contains integers N and M.
Next M lines contain connected junction pairs.
Last line contains source and destination.
Output Format
Print YES if route exists, otherwise NO.
Constraints
1 ≤ N ≤ 10^5
1 ≤ M ≤ 2×10^5
Sample Input
5 4
1 2
2 3
3 4
4 5
1 5
Sample Output
YES



Program:

import java.util.*;

public class traffic {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int n = sc.nextInt();
        int m = sc.nextInt();

        ArrayList<ArrayList<Integer>> graph = new ArrayList<>();

        for (int i = 0; i < n; i++) {
            graph.add(new ArrayList<>());
        }

        for (int i = 0; i < m; i++) {
            int u = sc.nextInt();
            int v = sc.nextInt();

            graph.get(u).add(v);
            graph.get(v).add(u);
        }

        int s = sc.nextInt();
        int d = sc.nextInt();

        boolean[] visited = new boolean[n];
        Queue<Integer> queue = new LinkedList<>();

        queue.add(s);
        visited[s] = true;

        while (!queue.isEmpty()) {
            int current = queue.poll();

            if (current == d) {
                break;
            }

            for (int neighbor : graph.get(current)) {
                if (!visited[neighbor]) {
                    visited[neighbor] = true;
                    queue.add(neighbor);
                }
            }
        }

        System.out.println(visited[d] ? "YES" : "NO");

        sc.close();
    }
}
