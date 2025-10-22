##unprotect method
## unprotect(self) {#}
Unprotects worksheet.
```python
def unprotect(self):
...
```
### Remarks
This method unprotects worksheet which is protected without password.
## unprotect(self, password) {#System.String}
Unprotects worksheet.
```python
def unprotect(self, password):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| password | System.String | Password |
### Remarks
If the worksheet is protected without a password, you can set a null value or blank string to password parameter.
### See Also
* module [`aspose.cells`](../../)
* class [`Worksheet`](/cells/python-net/aspose.cells/worksheet)
