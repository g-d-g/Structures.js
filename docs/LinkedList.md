# LinkedList

> [Wikipedia Article](http://en.wikipedia.org/wiki/Linked_list)

## Example

```javascript
var tree = new Structures.LinkedList([1, 2, 3, 4, 5, 6, 7, 8, 9]);

tree.filter(function(node, index, list){
  return Math.sqrt(node.getValue()) % 1 === 0;
});
tree = tree.map(function(node, index, list){
  return Math.sqrt(node.getValue());
});

console.log(tree.toArray());
```

## Methods

All methods meet [MDN Array](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array) specifications.

* Constructors
  * `LinkedList()`
  * `LinkedList([objects...])`
* `.push(object)`
* `.get(index)`
* `.remove(index)`
* `.length()`
* `.clear()`
* `.clone()`
* `.toArray()`
* `.traverse(function)`
  * Iterates over the list, calling function with the node, index, and list. Any values returned by function stop the traversal and are returned by the traversal.
* `.map(function)`
* `.filter(function)`
* `.splice(index, deleteAmount)`
* `.slice(start, end)`
* `.indexOf(value)`
* `.lastIndexOf(value)`