##add_identify method
## add_identify(self, range_index, page_item_index) {#int-list}
Sets which item label in each page field to use to identify the data range.
The pageItemIndex.Length must be equal to PageFieldCount, so please add the page field first.
```python
def add_identify(self, range_index, page_item_index):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| range_index | int | The consolidation data range index. |
| page_item_index | list | The page item index in the each page field.
### See Also
* module [`aspose.cells.pivot`](../../)
* class [`PivotPageFields`](/cells/python-net/aspose.cells.pivot/pivotpagefields)
