# Lec-2 01.04.2017

## Dynamic connectivity problem

> Component - one or more elements are connected to each other

# Union-find algorithm

Represent elements and conections betwin them in array
where index is element number (name) and value is component to which it belongs

```
 1 2 3 4 5   <= elements indexes
[1,1,3,5,5]  <= component name
```
here we have three components 
* 1 and 2
* 3
* 4 and 5

Union-find (uf) should support methods:

* `.connect(a,  d)` should conect two elements in one component
* `.isConnected(a,  d)` should return (boolean) ansver are two elements connected (in the same component / is there path from `a` to `b`)
* `.count()` should return number of components
* `.component(a)` should return component name or `undefined` if element not exist

### Examples

```javascript
uf.connect(1, 2); // elements => [undefined, 2, 2]
uf.isConnected(1,2); // true
uf.count(); // 1
uf.component(1); // 2

uf.connect(2, 3); // elements => [undefined, 3, 3, 3]
uf.isConnected(1,3); // true
uf.count(); // 1

uf.connect(0, 4); // elements => [4, 3, 3, 3, 4]
uf.connect(5, 0); // elements => [4, 3, 3, 3, 4, 4]
uf.isConnected(1,3); // true
uf.count(); // 2

uf.connect(7, 0); // elements => [4, 3, 3, 3, 4, 4, undefined, 4]
uf.isConnected(1,7); // false
uf.isConnected(7,6); // false
uf.count(); // 2

uf.connect(8, 9); // elements => [4, 3, 3, 3, 4, 4, undefined, 4, 9, 9]
uf.count(); // 3

uf.component(4); // 4 
uf.component(1); // 3 
uf.component(10); // undefined
```

## Home work

1. implement `uf.count()` method
1. implement `uf.component()` method
1. check test coverage for union-find (are you sure that your code work properly in different situations)