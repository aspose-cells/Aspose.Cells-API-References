##set_even_footer method
## set_even_footer(self, section, footer_script) {#int-System.String}
Sets a script formatting the even page footer of an Excel file.
Only effect in Excel 2007 when IsHFDiffOddEven is true.
```python
def set_even_footer(self, section, footer_script):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| section | int | 0: Left Section, 1: Center Section, 2: Right Section. |
| footer_script | System.String | Footer format script. |
### See Also
* module [`aspose.cells`](../../)
* class [`PageSetup`](/cells/python-net/aspose.cells/pagesetup)
