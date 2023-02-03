---
title: evaluated_page_count property
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 30
url: /python-net/aspose.cells.rendering/workbookprintingpreview/evaluated_page_count/
is_root: false
---

## evaluated_page_count property


Evaluate the total page count of this workbook

### Example 


The following code shows the fastest way to get page count of a workbook.

```python
from aspose.cells import Workbook
from aspose.cells.rendering import ImageOrPrintOptions, WorkbookPrintingPreview

workbook = Workbook("Book1.xlsx")
workbookPrintingPreview = WorkbookPrintingPreview(workbook, ImageOrPrintOptions())
# fastest way to get page count especailly when there are massive data in workbook.
print(workbookPrintingPreview.evaluated_page_count)

```

### See Also
* module [aspose.cells.rendering](../../)
* class [WorkbookPrintingPreview](/cells/python-net/aspose.cells.rendering/workbookprintingpreview)
