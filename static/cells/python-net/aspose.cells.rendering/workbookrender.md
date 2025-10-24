##WorkbookRender class
## WorkbookRender class
Represents a Workbook render.
The constructor of this class , must be used after modification of pagesetup, cell style.
The WorkbookRender type exposes the following members:
### Constructors
| Constructor | Description |
| :- | :- |
| [`__init__(self, workbook, options)`](/cells/python-net/aspose.cells.rendering/workbookrender/__init__/#aspose.cells.workbook-aspose.cells.rendering.imageorprintoptions) | The construct of WorkbookRender |
### Properties
| Property | Description |
| :- | :- |
| [page_count](/cells/python-net/aspose.cells.rendering/workbookrender/page_count) | Gets the total page count of workbook. |
### Methods
| Method | Description |
| :- | :- |
| [`to_image(self, stream)`](/cells/python-net/aspose.cells.rendering/workbookrender/to_image/#io.rawiobase) | Render whole workbook as Tiff Image to stream. |
| [`to_image(self, filename)`](/cells/python-net/aspose.cells.rendering/workbookrender/to_image/#system.string) | Render whole workbook as Tiff Image to a file. |
| [`to_image(self, page_index, file_name)`](/cells/python-net/aspose.cells.rendering/workbookrender/to_image/#int-system.string) | Render certain page to a file. |
| [`to_image(self, page_index, stream)`](/cells/python-net/aspose.cells.rendering/workbookrender/to_image/#int-io.rawiobase) | Render certain page to a stream. |
| [`to_printer(self, printer_name)`](/cells/python-net/aspose.cells.rendering/workbookrender/to_printer/#system.string) | Render workbook to Printer |
| [`to_printer(self, printer_name, job_name)`](/cells/python-net/aspose.cells.rendering/workbookrender/to_printer/#system.string-system.string) | Render workbook to Printer |
| [`to_printer(self, printer_settings)`](/cells/python-net/aspose.cells.rendering/workbookrender/to_printer/#aspose.pydrawing.printing.printersettings) | Render workbook to Printer |
| [`to_printer(self, printer_settings, job_name)`](/cells/python-net/aspose.cells.rendering/workbookrender/to_printer/#aspose.pydrawing.printing.printersettings-system.string) | Render workbook to Printer |
| [`to_printer(self, printer_name, print_page_index, print_page_count)`](/cells/python-net/aspose.cells.rendering/workbookrender/to_printer/#system.string-int-int) | Render workbook to Printer |
| [`get_page_size_inch(self, page_index)`](/cells/python-net/aspose.cells.rendering/workbookrender/get_page_size_inch/#int) | Get page size in inch of output image. |
| [`custom_print(self, next_page_after_print, print_page_event_args)`](/cells/python-net/aspose.cells.rendering/workbookrender/custom_print/#bool-aspose.pydrawing.printing.printpageeventargs) | Client can control page setting of printer when print each page using this function. |
| [`dispose(self)`](/cells/python-net/aspose.cells.rendering/workbookrender/dispose/#) | Releases resources created and used for rendering. |
### Remarks
### See Also
* module [`aspose.cells.rendering`](..)
