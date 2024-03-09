
---
- author : Daeyang-Kim
- created : 2024-03-03 16:22
- last_updated : 2024-03-03 16:22
- tags : #Literature #Algorithm
---

# BFS (Breadth-First Search)

## *주제*

너비 우선 탐색에 대해서 정리한다.
Java로 구현

## *정리*

```java

import java.util.LinkedList;
import java.util.Queue;

public class StudyBFS{
	static String bfs(int start , int[][] graph , boolean[] visited)
	{
		StringBuilder sb = new StringBuilder();
		Queue<Integer> q = new LinkedList<Integer>();

		q.offer(start);

		visited[start] = fals;

		while(!q.isEmpty())
		{
			int nodeIndex = q.poll();
			sb.append(nodeIndex + " -> ");
			for(int i = 0 ; i < graph[nodeIndex].length ; i++)
			{
				int temp = graph[nodeIndex][i];
				if(!visited[temp])
				{
					visited[temp] = true;
					q.offer(temp);
				}
			}
		}

		return sb.toString();
	}

	public static void main(String[] args)
	{
		int[][] graph = {{}, {2,3,8}, {1,6,8}, {1,5}, {5,7}, {3,4,7}, {2}, {4,5}, {1,2}};

		boolean[] visited = new boolean[9];

		System.out.println(bfs(1 , graph , visited));
	}
}


```

## *참고문헌*

- [https://codingnojam.tistory.com/41](https://codingnojam.tistory.com/41)

---

## *Link*
