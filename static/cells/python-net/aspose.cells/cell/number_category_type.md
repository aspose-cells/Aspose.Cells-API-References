##number_category_type property
## number_category_type property
Represents the category type of this cell's number formatting.
### Remarks
When cell's formatting pattern is combined with conditional formatting patterns,
then the returned type is corresponding to the part which is used for current value of this cell.
For example, if the formatting pattern for this cell is "#,##0;(#,##0);"-";@",
then when cell's value is numeric and not 0, the returned type is [`NumberCategoryType.NUMBER`](/cells/python-net/aspose.cells/numbercategorytype#NUMBER);
When cell's value is 0 or not numeric value, the returned type is [`NumberCategoryType.TEXT`](/cells/python-net/aspose.cells/numbercategorytype#TEXT).
### Definition:
```python
@property
def number_category_type(self):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`Cell`](/cells/python-net/aspose.cells/cell)
* class [`NumberCategoryType`](/cells/python-net/aspose.cells/numbercategorytype)
