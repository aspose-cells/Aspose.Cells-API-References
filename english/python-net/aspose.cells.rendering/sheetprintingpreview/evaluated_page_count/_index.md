---
title: evaluated_page_count property
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 30
url: /python-net/aspose.cells.rendering/sheetprintingpreview/evaluated_page_count/
is_root: false
---

## evaluated_page_count property


Evaluate the total page count of this worksheet
### Example 


The following code shows the fastest way to get page count of a worksheet.

```
from aspose.cells import Workbook
from aspose.cells.rendering import ImageOrPrintOptions, SheetPrintingPreview

workbook = Workbook("Book1.xlsx")
sheetPrintingPreview = SheetPrintingPreview(workbook.worksheets[0], ImageOrPrintOptions())

# fastest way to get page count especailly when there are massive data in worksheet.
print(sheetPrintingPreview.evaluated_page_count)

```

### See Also
* module [aspose.cells.rendering](../../)
* class [SheetPrintingPreview](/cells/python-net/aspose.cells.rendering/sheetprintingpreview)
