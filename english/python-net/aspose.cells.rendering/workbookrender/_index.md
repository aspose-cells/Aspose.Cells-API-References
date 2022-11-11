---
title: WorkbookRender
second_title: Aspose.Cells for Python via .NET API Reference
description: 
type: docs
weight: 130
url: /cells/python-net/aspose.cells.rendering/workbookrender/
---

## WorkbookRender class

Represents a Workbook render. <br/>            The constructor of this class , must be used after modification of pagesetup, cell style.

The WorkbookRender type exposes the following members:
## Constructors
| Name | Description |
| :- | :- |
|WorkbookRender(workbook, options)|Initializes a new instance of the WorkbookRender class|
## Properties
| Name | Description |
| :- | :- |
|page_count|Gets the total page count of workbook.|
## Methods
| Name | Description |
| :- | :- |
|to_image(stream)|Render whole workbook as Tiff Image to stream.|
|to_image(filename)|Render whole workbook as Tiff Image to a file.|
|to_image(page_index, file_name)|Render certain page to a file.|
|to_image(page_index, stream)|Render certain page to a stream.|
|to_printer(printer_name)|Render workbook to Printer|
|to_printer(printer_name, job_name)|Render workbook to Printer|
|to_printer(printer_settings)|Render workbook to Printer|
|to_printer(printer_settings, job_name)|Render workbook to Printer|
|to_printer(printer_name, print_page_index, print_page_count)|Render workbook to Printer|
|get_page_size(page_index)|Get page size of output image. The size unit is in pixel.|
|get_page_size_inch(page_index)|Get page size in inch of output image.|
|custom_print(next_page_after_print, print_page_event_args)|Client can control page setting of printer when print each page using this function.|

### See Also

* namespace [aspose.cells.rendering](/cells/python-net/aspose.cells.rendering/)
* assembly [Aspose.Cells](/cells/python-net/)

