##set_even_header method
## set_even_header(self, section, header_script) {#int-System.String}
Sets a script formatting the even page header of an Excel file.
Only effect in Excel 2007 when IsHFDiffOddEven is true.
```python
def set_even_header(self, section, header_script):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| section | int | 0: Left Section, 1: Center Section, 2: Right Section. |
| header_script | System.String | Header format script. |
### See Also
* module [`aspose.cells`](../../)
* class [`PageSetup`](/cells/python-net/aspose.cells/pagesetup)
