##table_style_type property
## table_style_type property
Gets and the built-in table style.
### Example
```python
from aspose.cells import Workbook
from aspose.cells.tables import TableStyleType
workbook = Workbook("Book1.xlsx")
tables = workbook.worksheets[0].list_objects
index = tables.add(0, 0, 9, 4, True)
table = tables[0]
table.table_style_type = TableStyleType.TABLE_STYLE_DARK2
workbook.save("TableStyle.xlsx")
```
### Definition:
```python
@property
def table_style_type(self):
...
@table_style_type.setter
def table_style_type(self, value):
...
```
### See Also
* module [`aspose.cells.tables`](../../)
* class [`ListObject`](/cells/python-net/aspose.cells.tables/listobject)
* class [`TableStyleType`](/cells/python-net/aspose.cells.tables/tablestyletype)
