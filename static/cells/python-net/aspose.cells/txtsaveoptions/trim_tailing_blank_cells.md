##trim_tailing_blank_cells property
## trim_tailing_blank_cells property
Indicates whether tailing blank cells in one row should be trimmed. Default is false.
### Remarks
When saving with LightCells mode and the [`TxtSaveOptions.export_area`](/cells/python-net/aspose.cells/txtsaveoptions#export_area) has not been specified,
this option takes no effect and one row will be extended to just the last cell provided by
the implementation [`TxtSaveOptions.light_cells_data_provider`](/cells/python-net/aspose.cells/txtsaveoptions#light_cells_data_provider)
### Definition:
```python
@property
def trim_tailing_blank_cells(self):
...
@trim_tailing_blank_cells.setter
def trim_tailing_blank_cells(self, value):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`TxtSaveOptions`](/cells/python-net/aspose.cells/txtsaveoptions)
