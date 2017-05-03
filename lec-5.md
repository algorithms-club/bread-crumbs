# Lec-4 29.04.2017

## Sorting algorithms

*Problem:* to arrange elements of the collection in order.
Good sorting algorithm able sort elements of any type, callback pattern can help to achieve that.
In any sorting algorithm, we should answer, is element `a` bigger than `b`
general syntax can look like:
```javascript
function compare(a,b) {
  if (a > b) {
    return 1;
  }

  if (a < b) {
    return -1;
  }

  return 0;
}

sort([3,6,2,7], compare)
```
in any time when sorting algorithm should know is the one element bigger than another it use compare function

### Selection sort
https://en.wikipedia.org/wiki/Selection_sort
https://www.youtube.com/watch?v=92BfuxHn2XE 

### Insertion sort
https://en.wikipedia.org/wiki/Insertion_sort
https://www.youtube.com/watch?v=8oJS1BMKE64

### Shell sort
https://en.wikipedia.org/wiki/Shellsort
https://www.youtube.com/watch?v=n4sk-SzGvZA


# Home work

1. Implement helper function
  * shuffle (should take collection and return in random order)
  * isSorted (should take collection and return boolean)
1. Implement Selection sort OR Insertion sort
2. Implement Shell sort

Optional 
1. Merge sort
2. Quick sort

