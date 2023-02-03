---
title: page_count property
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 310
url: /python-net/aspose.cells/pdfsaveoptions/page_count/
is_root: false
---

## page_count property


Gets or sets the number of pages to save.

### Remarks 


Default is System.Int32.MaxValue which means all pages will be rendered..

### Example 


The following example shows how to render a range of pages (3 and 4) in a Microsoft Excel file to PDF.

```python
from aspose.cells import PdfSaveOptions, Workbook

# Open an Excel file
wb = Workbook("Book1.xlsx")
options = PdfSaveOptions()
# Print only Page 3 and Page 4 in the output PDF
# Starting page index (0-based index)
options.page_index = 3
# Number of pages to be printed
options.page_count = 2
# Save the PDF file
wb.save("output.pdf", options)

```

### See Also
* module [aspose.cells](../../)
* class [PdfSaveOptions](/cells/python-net/aspose.cells/pdfsaveoptions)
