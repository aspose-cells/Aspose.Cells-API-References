##update_linked_data_source method
## update_linked_data_source(self, external_workbooks) {#list}
If this workbook contains external links to other data source,
Aspose.Cells will attempt to retrieve the latest data from give sources.
```python
def update_linked_data_source(self, external_workbooks):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| external_workbooks | list | Workbooks that will be used to update data of external links referenced by this workbook.
### Remarks
If corresponding external link cannot be found for one workbook, then this workbook will be ignored.
So when you set a formula later with one new external link which you intend to make the ignored workbook
be linked to it, the link cannot be performed until you call this this method again with those workbooks.
### See Also
* module [`aspose.cells`](../../)
* class [`Workbook`](/cells/python-net/aspose.cells/workbook)
