---
title: printing_page_type property
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 350
url: /python-net/aspose.cells/pdfsaveoptions/printing_page_type/
is_root: false
---

## printing_page_type property


Indicates which pages will not be printed.

### Remarks 


If content in the sheet is sparse, there will be some pages are totally blank in the output pdf file.
If you don't want these blank pages, you can use this option to omit them.

### Example 


The following code omits blank pages or pages which only contains some style content like cell background, borders.

```python
from aspose.cells import PdfSaveOptions, PrintingPageType, Workbook

wb = Workbook("Book1.xlsx")
pdfSaveOptions = PdfSaveOptions()
# ignore blank pages
pdfSaveOptions.printing_page_type = PrintingPageType.IGNORE_BLANK
wb.save("output_ignore_blank_page.pdf", pdfSaveOptions)
# ignore blank pages and pages which only contains some style content like cell background
pdfSaveOptions.printing_page_type = PrintingPageType.IGNORE_STYLE
wb.save("output_ignore_blank_and_style_page.pdf", pdfSaveOptions)

```

### See Also
* module [aspose.cells](../../)
* class [PdfSaveOptions](/cells/python-net/aspose.cells/pdfsaveoptions)
