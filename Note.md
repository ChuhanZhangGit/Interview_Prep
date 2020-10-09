### Corner cases

- Check for empty set, matrix, string, list.
- Use max/min on empty iterable
- List, array index a[i, j +1] for i to j.
- Update the value without checking if current value is better than previous.
- Look out for >= vs >; large equal vs strictly larger


### Graph Errors
- DFS / BFS 
Before or during traversal need to keep track to visited nodes, prevent revist node, to ***avoid LOOPs and Overflows***.

- BFS: Update the visited flag immediate after the node have been put into queue. If not but update flag after polling the node from the queue, in case current level's nodes has parent/children relation with each other, some nodes will be visited multiple times before the visited flag gets updated.

---

### Syntax Errors
#### 2D data structure
- Incompatible types
```
List<List<Integer>> output = new ArrayList<ArrayList<Integer>>();
```
Should be 
```
List<List<Integer>> output = new ArrayList<List<Integer>>();
```
Because List<List<Integer>> can add Other concrete object list into it e.g. LinkedList. But ArrayList<ArrayList<Integer>>, only ArrayList can be added to it.

