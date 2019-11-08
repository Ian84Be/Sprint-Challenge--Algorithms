#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

* a) 0(n)
	* this has a linear time complexity because the while loop runs for every value of n
	* this is pretty good


* b) 0(n log n)
	* this has an outer loop that runs for every value of n, and an inner loop that runs for log(n)
	* this is pretty bad, but not terrible


* c) 0(n)
	* linear time complexity, the function recurses once for every value of n

## Exercise II

``` 
howHigh(min=1, max=n):
	mid = n // 2
	if eggDrop(mid) == broken:
		howHigh(1, mid)
	else:
		howHigh(mid, n)
```

* we could start the first floor and drop an egg until it breaks, that would be 0(n) runtime, not bad, not great, breaks a lot of eggs
* better to split the work into chunks, start at the middle floor, if it breaks, you can eliminate half of n already so this would be 0(log n) runtime, which is about as good as it gets
