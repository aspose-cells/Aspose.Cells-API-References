##set_first_page_header method
## set_first_page_header(self, section, header_script) {#int-System.String}
Sets a script formatting the first page header of an Excel file.
Only effect in Excel 2007 when IsHFDiffFirst is true.
```python
def set_first_page_header(self, section, header_script):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| section | int | 0: Left Section, 1: Center Section, 2: Right Section. |
| header_script | System.String | Header format script. |
### See Also
* module [`aspose.cells`](../../)
* class [`PageSetup`](/cells/python-net/aspose.cells/pagesetup)
