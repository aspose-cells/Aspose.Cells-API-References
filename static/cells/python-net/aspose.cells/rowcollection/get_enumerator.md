##get_enumerator method
## get_enumerator(self, reversed, sync) {#bool-bool}
Gets an enumerator that iterates rows through this collection
### Returns
The row enumerator which will traverse all existing rows in this collection.
```python
def get_enumerator(self, reversed, sync):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| reversed | bool | whether enumerate rows in reversed order |
| sync | bool | whether the returned enumerator should check the modification of row collection
### Remarks
If the row collection will be modified(by operations that may cause new Row be instantiated or
existing Row be removed) during the traversal with the enumerator,
synchronized enumerator should be used instead of normal enumerator so that the traversal can continue
from the position just after the one has been traversed by the last MoveNext().
However, together with the advantage that no element be skipped or traversed repeatedly,
the disadvantage for synchronized enumerator is that the performance will be degraded a bit
when comparing with normal enumerator.
### See Also
* module [`aspose.cells`](../../)
* class [`RowCollection`](/cells/python-net/aspose.cells/rowcollection)
