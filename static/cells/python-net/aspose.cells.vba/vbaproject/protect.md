##protect method
## protect(self, islocked_for_viewing, password) {#bool-System.String}
Protects or unprotects this VBA project.
```python
def protect(self, islocked_for_viewing, password):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| islocked_for_viewing | bool | indicates whether locks project for viewing. |
| password | System.String | If the value is null, unprotects this VBA project, otherwise projects the this VBA project. |
### Remarks
If islockedForViewing is true, the password could not be null.
### See Also
* module [`aspose.cells.vba`](../../)
* class [`VbaProject`](/cells/python-net/aspose.cells.vba/vbaproject)
