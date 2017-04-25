# Lec-4 22.04.2017

## Basyc data structure

### Array

Random access memory, it requires single, not fragmented sequence of memory cells, variable with array point to the first element with index 0. 
Each element goes one after another in memory, so it possible te calculate the address of any index in the array if we know the address of 0th element.

Incase when 0 element should be deleted or insert new element at the bigining need to shift all aelements

In case with dynamic length array, under the hood created array with defined length and every time there are no free space in the array, it should find new place in memory to copy current elements + new one.

https://en.wikipedia.org/wiki/Array_data_structure

### Linked list

Each element of linked list have value and link to next element in the list.
When new element adding to list, it finds place in memory to save one value plus link to the next element and change the link of the previous element to point to the new one.

Pay attention to complexity of basics operations with linked list and array in wikipedia

https://en.wikipedia.org/wiki/Linked_list

### Stack and Queue

Collections of elements have two method `inser` nad `get`

in the stack, insertion and getting elements should be the same no matter at the start of the collection or at the end

in queue insert a new element to the beginning and get an element from the end


https://en.wikipedia.org/wiki/Stack_(abstract_data_type)

https://en.wikipedia.org/wiki/Queue_(abstract_data_type)


## How to Review

- you should understand the code.
- code style should be the same during all code and not mixing different syles
- namein of variables should be meaningful
- all methods should be cover by test
- tests should passing
- code should be pretty and clean
    - no useless variables
    - no useless or redundant comments

# Home work

1. Implement linked list
2. Implement Stack and Queue base on linked list 
