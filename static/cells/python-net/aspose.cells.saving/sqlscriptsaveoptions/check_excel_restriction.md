##check_excel_restriction property
## check_excel_restriction property
Whether check restriction of excel file when user modify cells related objects.
For example, excel does not allow inputting string value longer than 32K.
When you input a value longer than 32K, it will be truncated.
### Definition:
```python
@property
def check_excel_restriction(self):
...
@check_excel_restriction.setter
def check_excel_restriction(self, value):
...
```
### See Also
* module [`aspose.cells.saving`](../../)
* class [`SqlScriptSaveOptions`](/cells/python-net/aspose.cells.saving/sqlscriptsaveoptions)
