---
title: WorkbookRender class
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 130
url: /python-net/aspose.cells.rendering/workbookrender/
is_root: false
---

## WorkbookRender class

Represents a Workbook render. 
The constructor of this class , must be used after modification of pagesetup, cell style.



The WorkbookRender type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [WorkbookRender(workbook, options)](/cells/python-net/aspose.cells.rendering/workbookrender/__init__/#Workbook-ImageOrPrintOptions) | The construct of WorkbookRender |


### Properties
| Property | Description |
| :- | :- |
| [page_count](/cells/python-net/aspose.cells.rendering/workbookrender/page_count) | Gets the total page count of workbook. |


### Methods
| Method | Description |
| :- | :- |
| [to_image(stream)](/cells/python-net/aspose.cells.rendering/workbookrender/to_image/#io.RawIOBase) | Render whole workbook as Tiff Image to stream. |
| [to_image(filename)](/cells/python-net/aspose.cells.rendering/workbookrender/to_image/#str) | Render whole workbook as Tiff Image to a file. |
| [to_image(page_index, file_name)](/cells/python-net/aspose.cells.rendering/workbookrender/to_image/#int-str) | Render certain page to a file. |
| [to_image(page_index, stream)](/cells/python-net/aspose.cells.rendering/workbookrender/to_image/#int-io.RawIOBase) | Render certain page to a stream. |
| [to_printer(printer_name)](/cells/python-net/aspose.cells.rendering/workbookrender/to_printer/#str) | Render workbook to Printer |
| [to_printer(printer_name, job_name)](/cells/python-net/aspose.cells.rendering/workbookrender/to_printer/#str-str) | Render workbook to Printer |
| [to_printer(printer_settings)](/cells/python-net/aspose.cells.rendering/workbookrender/to_printer/#aspose.pydrawing.printing.PrinterSettings) | Render workbook to Printer |
| [to_printer(printer_settings, job_name)](/cells/python-net/aspose.cells.rendering/workbookrender/to_printer/#aspose.pydrawing.printing.PrinterSettings-str) | Render workbook to Printer |
| [to_printer(printer_name, print_page_index, print_page_count)](/cells/python-net/aspose.cells.rendering/workbookrender/to_printer/#str-int-int) | Render workbook to Printer |
| [get_page_size_inch(page_index)](/cells/python-net/aspose.cells.rendering/workbookrender/get_page_size_inch/#int) | Get page size in inch of output image. |
| [custom_print(next_page_after_print, print_page_event_args)](/cells/python-net/aspose.cells.rendering/workbookrender/custom_print/#bool-aspose.pydrawing.printing.PrintPageEventArgs) | Client can control page setting of printer when print each page using this function. |


### Remarks 



### See Also

* module [aspose.cells.rendering](../)
