##merged_cells_shrink_type property
## merged_cells_shrink_type property
Indicates how to process merged cells when deleting blank rows/columns.
### Remarks
For [`MergedCellsShrinkType.KEEP_HEADER_ONLY`](/cells/python-net/aspose.cells/mergedcellsshrinktype#KEEP_HEADER_ONLY), all cells in it will be taken as blank except the non-blank top-left cell. It is the default value of this property.
For [`MergedCellsShrinkType.NONE`](/cells/python-net/aspose.cells/mergedcellsshrinktype#NONE), all cells in it will be taken as non-blank.
For [`MergedCellsShrinkType.SHRINK_TO_FIT`](/cells/python-net/aspose.cells/mergedcellsshrinktype#SHRINK_TO_FIT), all cells outside the content display area will be taken as blank.
### Definition:
```python
@property
def merged_cells_shrink_type(self):
...
@merged_cells_shrink_type.setter
def merged_cells_shrink_type(self, value):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`DeleteBlankOptions`](/cells/python-net/aspose.cells/deleteblankoptions)
* class [`MergedCellsShrinkType`](/cells/python-net/aspose.cells/mergedcellsshrinktype)
