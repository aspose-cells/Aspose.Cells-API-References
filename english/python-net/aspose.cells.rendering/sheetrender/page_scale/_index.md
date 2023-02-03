---
title: page_scale property
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 90
url: /python-net/aspose.cells.rendering/sheetrender/page_scale/
is_root: false
---

## page_scale property


Gets calculated page scale of the sheet.
Returns the set scale if [PageSetup.zoom](/cells/python-net/aspose.cells/pagesetup#zoom) is set. Otherwise, returns the calculated scale according to [PageSetup.fit_to_pages_wide](/cells/python-net/aspose.cells/pagesetup#fit_to_pages_wide) and [PageSetup.fit_to_pages_tall](/cells/python-net/aspose.cells/pagesetup#fit_to_pages_tall).

### Example 


```python
from aspose.cells import Workbook
from aspose.cells.rendering import ImageOrPrintOptions, SheetRender

wb = Workbook("Book1.xlsx")
sheetRender = SheetRender(wb.worksheets[0], ImageOrPrintOptions())
# Gets calculated page scale of the sheet.
pageScale = sheetRender.page_scale

```

### See Also
* module [aspose.cells.rendering](../../)
* class [SheetRender](/cells/python-net/aspose.cells.rendering/sheetrender)
