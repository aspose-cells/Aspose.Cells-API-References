##copy_to method
## copy_to(self, array) {#list}
Copies the entire array list to a compatible one-dimensional array list, starting at the beginning of the target array list.
```python
def copy_to(self, array):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| array | list | The one-dimensional array list that is the destination of the elements copied array list. The array list must have zero-based indexing. |
## copy_to(self, index, array, array_index, count) {#int-list-int-int}
Copies a range of elements from the array list to a compatible one-dimensional array list, starting at the specified index of the target array list.
```python
def copy_to(self, index, array, array_index, count):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| index | int | The zero-based index in the source array list at which copying begins. |
| array | list | The one-dimensional array list that is the destination of the elements copied from array list. The array list must have zero-based indexing. |
| array_index | int | The zero-based index in array list at which copying begins. |
| count | int | The number of elements to copy. |
### See Also
* module [`aspose.cells.querytables`](../../)
* class [`PowerQueryFormulaCollection`](/cells/python-net/aspose.cells.querytables/powerqueryformulacollection)
