##use_sheet_name property
## use_sheet_name property
Whether builds the file path with sheet name instead of sheet index. Default value is false.
### Remarks
The sheet name will never be rebuilt automatically.
So when set it to true, please make sure there is no special sheet name
that can cause invalid file path or name.
### Definition:
```python
@property
def use_sheet_name(self):
...
@use_sheet_name.setter
def use_sheet_name(self, value):
...
```
### See Also
* module [`aspose.cells.lowcode`](../../)
* class [`LowCodeSaveOptionsProviderOfAssembling`](/cells/python-net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling)
