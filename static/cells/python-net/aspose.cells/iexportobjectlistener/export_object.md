##export_object method
## export_object(self, e) {#aspose.cells.ExportObjectEvent}
Export one object.
### Returns
The information about the result of exporting object.
* For exporting objects when export workbook to HTML format,
the result is URL string to access the saved Image from the html file which contains this exported object.
```python
def export_object(self, e):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| e | aspose.cells.ExportObjectEvent | The event triggered when one object needs to be exported. |
### See Also
* module [`aspose.cells`](../../)
* class [`IExportObjectListener`](/cells/python-net/aspose.cells/iexportobjectlistener)
