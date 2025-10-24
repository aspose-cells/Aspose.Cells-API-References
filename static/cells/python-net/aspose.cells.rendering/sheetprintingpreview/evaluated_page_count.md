##evaluated_page_count property
## evaluated_page_count property
Evaluate the total page count of this worksheet
### Example
The following code shows the fastest way to get page count of a worksheet.
```python
from aspose.cells import Workbook
from aspose.cells.rendering import ImageOrPrintOptions, SheetPrintingPreview
workbook = Workbook("Book1.xlsx")
sheetPrintingPreview = SheetPrintingPreview(workbook.worksheets[0], ImageOrPrintOptions())
# fastest way to get page count especailly when there are massive data in worksheet.
print(sheetPrintingPreview.evaluated_page_count)
```
### Definition:
```python
@property
def evaluated_page_count(self):
...
```
### See Also
* module [`aspose.cells.rendering`](../../)
* class [`SheetPrintingPreview`](/cells/python-net/aspose.cells.rendering/sheetprintingpreview)
