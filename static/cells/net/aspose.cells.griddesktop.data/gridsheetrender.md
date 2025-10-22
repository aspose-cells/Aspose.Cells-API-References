##Class GridSheetRender
Aspose.Cells.GridDesktop.Data.GridSheetRender class. Represents a worksheet render which can render worksheet to various images such as BMP PNG JPEG TIFF.. The constructor of this class  must be used after modification of pagesetup cell style
## GridSheetRender class
Represents a worksheet render which can render worksheet to various images such as (BMP, PNG, JPEG, TIFF..) The constructor of this class , must be used after modification of pagesetup, cell style.
```csharp
public class GridSheetRender
```
## Constructors
| Name | Description |
| --- | --- |
| [GridSheetRender](gridsheetrender/)(Worksheet, GridImageOrPrintOptions) | the construct of SheetRender, need worksheet and ImageOrPrintOptions as params |
## Properties
| Name | Description |
| --- | --- |
| [PageCount](../../aspose.cells.griddesktop.data/gridsheetrender/pagecount/) { get; } | Gets the total page count of current worksheet. |
| [PageScale](../../aspose.cells.griddesktop.data/gridsheetrender/pagescale/) { get; } | Gets calculated page scale of the sheet. |
## Methods
| Name | Description |
| --- | --- |
| [GetPageSizeInch](../../aspose.cells.griddesktop.data/gridsheetrender/getpagesizeinch/)(int) | Get page size in inch of output image. |
| [ToImage](../../aspose.cells.griddesktop.data/gridsheetrender/toimage/#toimage)(int) | Render certain page to a Bitmap object. |
| [ToImage](../../aspose.cells.griddesktop.data/gridsheetrender/toimage/#toimage_3)(int, Stream) | Render certain page to a stream. |
| [ToImage](../../aspose.cells.griddesktop.data/gridsheetrender/toimage/#toimage_4)(int, string) | Render certain page to a file. |
| [ToImage](../../aspose.cells.griddesktop.data/gridsheetrender/toimage/#toimage_1)(int, Graphics, float, float) | Render certain page to a Graphics |
| [ToImage](../../aspose.cells.griddesktop.data/gridsheetrender/toimage/#toimage_2)(int, Graphics, float, float, float, float) | Render certain page to a Graphics |
| [ToPrinter](../../aspose.cells.griddesktop.data/gridsheetrender/toprinter/#toprinter)(PrinterSettings) | Render worksheet to Printer |
| [ToPrinter](../../aspose.cells.griddesktop.data/gridsheetrender/toprinter/#toprinter_2)(string) | Render worksheet to Printer |
| [ToPrinter](../../aspose.cells.griddesktop.data/gridsheetrender/toprinter/#toprinter_1)(PrinterSettings, string) | Render worksheet to Printer |
| [ToPrinter](../../aspose.cells.griddesktop.data/gridsheetrender/toprinter/#toprinter_3)(string, string) | Render worksheet to Printer |
| [ToTiff](../../aspose.cells.griddesktop.data/gridsheetrender/totiff/#totiff)(Stream) | Render whole worksheet as Tiff Image to stream. |
| [ToTiff](../../aspose.cells.griddesktop.data/gridsheetrender/totiff/#totiff_1)(string) | Render whole worksheet as Tiff Image to a file. |
### See Also
* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)
