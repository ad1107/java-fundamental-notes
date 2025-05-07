## Selection Sort: Search-And-Swap:
- Find smallest element, exchange `a[0]`
- Then find smallest element from 1 to end, exchange `a[1]`
- n-1 passes.
```java
public void selectionSort(){
	int maxPos, max;
	
	for (int i = 0; i < a.length - 1; i++){
		max = a[i];
		maxPos = i;
		for (int j = i + 1; j < a.length; j++){
			if (max < a[j]) {
				max = a[j];
				maxPos = j;
			}
		}
		swap(i, maxPos);
	}
} 
```

## Insertion Sort: 
- Left half: Sorted
- Right half: Unsorted - each element will move and insert to correct location in left half.
- n-1.

## Mergesort: Recursive
- Break array 2 halves
- Mergesort left half
- Mergesort right half
- Merge to sorted.

## Binary search:
```java
if (low > high) return -1 // Base case
else {
	mid = (low + high) / 2;
	if (key == a[mid]) return mid;
	else if (key < mid) binSearch(low, mid-1);
	else binSearch(mid+1, high);
}
```
