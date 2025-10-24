##get_enumerator method
## get_enumerator(self, reversed, sync) {#bool-bool}
Gets an enumerator that iterates cells through this row.
### Returns
The cells enumerator which will traverse all existing cells in this row.
```python
def get_enumerator(self, reversed, sync):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| reversed | bool | whether enumerate cells in reversed order |
| sync | bool | whether the returned enumerator should check the modification of cells in this row
### Remarks
If the row will be modified(by operations that may cause new Cell be instantiated or
existing Cell be removed) during the traversal with the enumerator,
synchronized enumerator should be used instead of normal enumerator so that the traversal can continue
from the position just after the one has been traversed by the last MoveNext().
However, together with the advantage that no element be skipped or traversed repeatedly,
the disadvantage for synchronized enumerator is that the performance will be degraded a bit
when comparing with normal enumerator.
### See Also
* module [`aspose.cells`](../../)
* class [`Row`](/cells/python-net/aspose.cells/row)
