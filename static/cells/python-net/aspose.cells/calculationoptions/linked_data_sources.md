##linked_data_sources property
## linked_data_sources property
Specifies the data sources for external links used in formulas.
### Remarks
Like [`Workbook.update_linked_data_source`](/cells/python-net/aspose.cells/workbook/update_linked_data_source), here you may specify
data sources for external links used in formulas to be calculated, especially those
used in INDIRECT function. For those external links used in INDIRECT function,
they are not taken as part of the external links of the workbook and cannot be updated
by [`Workbook.update_linked_data_source`](/cells/python-net/aspose.cells/workbook/update_linked_data_source).
The match of those workbooks with external links is determined by [`Workbook.file_name`](/cells/python-net/aspose.cells/workbook#file_name)
and [`ExternalLink.data_source`](/cells/python-net/aspose.cells/externallink#data_source). So please make sure [`Workbook.file_name`](/cells/python-net/aspose.cells/workbook#file_name) has
been specified with the proper value(generally it should be same with corresponding
[`ExternalLink.data_source`](/cells/python-net/aspose.cells/externallink#data_source)) for every workbook so they can be linked as expected.
### Definition:
```python
@property
def linked_data_sources(self):
...
@linked_data_sources.setter
def linked_data_sources(self, value):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`CalculationOptions`](/cells/python-net/aspose.cells/calculationoptions)
