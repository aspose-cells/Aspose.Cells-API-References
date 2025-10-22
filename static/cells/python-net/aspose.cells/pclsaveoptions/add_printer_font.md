##add_printer_font method
## add_printer_font(self, font_full_name, font_pcl_name) {#System.String-System.String}
Adds information about font that is already added to the printer by manufacturer.
```python
def add_printer_font(self, font_full_name, font_pcl_name):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| font_full_name | System.String | Full name of the font (e.g. "Times New Roman Bold Italic") used in the source file. |
| font_pcl_name | System.String | Name of the font that will be used in the output Pcl document. |
### Remarks
There are 52 fonts that are to be built in any printer according to Pcl specification.
However manufactures can add some other fonts to their devices.
### See Also
* module [`aspose.cells`](../../)
* class [`PclSaveOptions`](/cells/python-net/aspose.cells/pclsaveoptions)
