# ADS - ASSIGNMENT 1 
There are my responses to the first assignment. 

## Task 1 

**Explanation**

You are given a number "n" and an array of "n" elements, write the function that returns minimum of them 


```
    public static int findMin(int[] arr, int n) {
        if (n==1)
            return arr[0];
        else {
            int min = findMin(arr, n-1);
            return Math.min(min, arr[n-1]);
        }
    }
``` 
  
    
## Task 2 

**Explanation** 

You are given a number "n" and an array of "n" elements, write the function that returns average of them. 


```
public double findAvg(int n, int[] nums) {
        double total = nums[0]; 
        for (int i = 1; i < n; i++) { 
            total += nums[i]; 
        }
        return total / n; 
    }
```

## Task 3 

**Explanation** 

You are given a number "n", write the function for checking whether "n" is prime. 

```
public boolean isPrime(int n) {
        int del = 0; // declaring a new value
        for (int i = 1; i < n; i++) {
            if (n % i == 0) { // check is the number divisible to others
                del++; //
            }
        }
        return del == 0;
    }
```

