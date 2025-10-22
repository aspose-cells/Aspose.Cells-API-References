##get_leafs method
## get_leafs(self) {#}
Get all cells which reference to this cell directly and need to be updated when this cell is modified.
### Returns
Enumerator to enumerate all dependents(Cell)
```python
def get_leafs(self):
...
```
### Remarks
NOTE: This class is now obsolete. Instead,
please use Cell.GetDependentsInCalculation(bool) to get all dependents in calculation chain.
This property will be removed 12 months later since May 2022.
Aspose apologizes for any inconvenience you may have experienced.
## get_leafs(self, recursive) {#bool}
Get all cells which will be updated when this cell is modified.
### Returns
Enumerator to enumerate all dependents(Cell)
```python
def get_leafs(self, recursive):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| recursive | bool | Whether returns those leafs that do not reference to this cell directly
### Remarks
NOTE: This class is now obsolete. Instead,
please use Cell.GetDependentsInCalculation(bool) to get all dependents in calculation chain.
This property will be removed 12 months later since May 2022.
Aspose apologizes for any inconvenience you may have experienced.
### See Also
* module [`aspose.cells`](../../)
* class [`Cell`](/cells/python-net/aspose.cells/cell)
