---
title: Class SheetRender
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Rendering.SheetRender class. Represents a worksheet render which can render worksheet to various images such as BMP PNG JPEG TIFF.. The constructor of this class  must be used after modification of pagesetup cell style
type: docs
url: /net/aspose.cells.rendering/sheetrender/
---
## SheetRender class

Represents a worksheet render which can render worksheet to various images such as (BMP, PNG, JPEG, TIFF..) The constructor of this class , must be used after modification of pagesetup, cell style.

```csharp
public class SheetRender
```

## Constructors

| Name | Description |
| --- | --- |
| [SheetRender](sheetrender/)(Worksheet, ImageOrPrintOptions) | the construct of SheetRender, need worksheet and ImageOrPrintOptions as params |

## Properties

| Name | Description |
| --- | --- |
| [PageCount](../../aspose.cells.rendering/sheetrender/pagecount/) { get; } | Gets the total page count of current worksheet. |
| [PageScale](../../aspose.cells.rendering/sheetrender/pagescale/) { get; } | Gets calculated page scale of the sheet. Returns the set scale if [`Zoom`](../../aspose.cells/pagesetup/zoom/) is set. Otherwise, returns the calculated scale according to [`FitToPagesWide`](../../aspose.cells/pagesetup/fittopageswide/) and [`FitToPagesTall`](../../aspose.cells/pagesetup/fittopagestall/). |

## Methods

| Name | Description |
| --- | --- |
| [CustomPrint](../../aspose.cells.rendering/sheetrender/customprint/)(bool, PrintPageEventArgs) | Client can control page setting of printer when print each page using this function. |
| [Dispose](../../aspose.cells.rendering/sheetrender/dispose/)() | Releases resources created and used for rendering. |
| [GetPageSizeInch](../../aspose.cells.rendering/sheetrender/getpagesizeinch/)(int) | Get page size in inch of output image. |
| [ToImage](../../aspose.cells.rendering/sheetrender/toimage/#toimage)(int) | Render certain page to a Bitmap object. |
| [ToImage](../../aspose.cells.rendering/sheetrender/toimage/#toimage_3)(int, Stream) | Render certain page to a stream. |
| [ToImage](../../aspose.cells.rendering/sheetrender/toimage/#toimage_4)(int, string) | Render certain page to a file. |
| [ToImage](../../aspose.cells.rendering/sheetrender/toimage/#toimage_1)(int, Graphics, float, float) | Render certain page to a Graphics |
| [ToImage](../../aspose.cells.rendering/sheetrender/toimage/#toimage_2)(int, Graphics, float, float, float, float) | Render certain page to a Graphics |
| [ToPrinter](../../aspose.cells.rendering/sheetrender/toprinter/#toprinter)(PrinterSettings) | Render worksheet to Printer |
| [ToPrinter](../../aspose.cells.rendering/sheetrender/toprinter/#toprinter_2)(string) | Render worksheet to Printer |
| [ToPrinter](../../aspose.cells.rendering/sheetrender/toprinter/#toprinter_1)(PrinterSettings, string) | Render worksheet to Printer |
| [ToPrinter](../../aspose.cells.rendering/sheetrender/toprinter/#toprinter_4)(string, string) | Render worksheet to Printer |
| [ToPrinter](../../aspose.cells.rendering/sheetrender/toprinter/#toprinter_3)(string, int, int) | (**Obsolete.**) Render worksheet to Printer |
| [ToTiff](../../aspose.cells.rendering/sheetrender/totiff/#totiff)(Stream) | Render whole worksheet as Tiff Image to stream. |
| [ToTiff](../../aspose.cells.rendering/sheetrender/totiff/#totiff_1)(string) | Render whole worksheet as Tiff Image to a file. |

### Examples

```csharp
// Called: SheetRender sr = new SheetRender(wb.Worksheets[0], new ImageOrPrintOptions());
public void Rendering_Type_SheetRender()
{
    Workbook wb = new Workbook(Constants.TemplatePath + "example.xlsx");

    PageSetup pageSetup = wb.Worksheets[0].PageSetup;
    pageSetup.PrintArea = "1:59";
    pageSetup.SetFitToPages(0, 1);

    SheetRender sr = new SheetRender(wb.Worksheets[0], new ImageOrPrintOptions());
    int zoom = (int)(sr.PageScale * 100 + 0.5);
    Assert.AreEqual(53, zoom);
}
```

### See Also

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


