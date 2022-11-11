---
title: SheetRender
second_title: Aspose.Cells for Python via .NET API Reference
description: 
type: docs
weight: 100
url: /python-net/aspose.cells.rendering/sheetrender/
---

## SheetRender class

Represents a worksheet render which can render worksheet to various images such as (BMP, PNG, JPEG, TIFF..)<br/>            The constructor of this class , must be used after modification of pagesetup, cell style.

The SheetRender type exposes the following members:
## Constructors
| Name | Description |
| :- | :- |
|SheetRender(worksheet, options)|Initializes a new instance of the SheetRender class|
## Properties
| Name | Description |
| :- | :- |
|page_count|Gets the total page count of current worksheet.|
|page_scale|Gets calculated page scale of the sheet.<br/>            Returns the set scale if [zoom](/python-net/aspose.cells/pagesetup/) is set. Otherwise, returns the calculated scale according to [fit_to_pages_wide](/python-net/aspose.cells/pagesetup/) and [fit_to_pages_tall](/python-net/aspose.cells/pagesetup/).|
## Methods
| Name | Description |
| :- | :- |
|to_image(page_index, file_name)|Render certain page to a file.|
|to_image(page_index, stream)|Render certain page to a stream.|
|to_tiff(stream)|Render whole worksheet as Tiff Image to stream.|
|to_tiff(filename)|Render whole worksheet as Tiff Image to a file.|
|to_printer(printer_name)|Render worksheet to Printer|
|to_printer(printer_name, job_name)|Render worksheet to Printer|
|to_printer(printer_settings)|Render worksheet to Printer|
|to_printer(printer_settings, job_name)|Render worksheet to Printer|
|to_printer(printer_name, print_page_index, print_page_count)|Render worksheet to Printer|
|get_page_size(page_index)|Get page size of output image. The size unit is in pixel.|
|get_page_size_inch(page_index)|Get page size in inch of output image.|
|custom_print(next_page_after_print, print_page_event_args)|Client can control page setting of printer when print each page using this function.|

### See Also

* namespace [aspose.cells.rendering](/python-net/aspose.cells.rendering/)
* assembly [Aspose.Cells](/python-net/)

