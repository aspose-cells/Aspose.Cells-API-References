---
title: Class WorkbookRender
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Rendering.WorkbookRender class. Represents a Workbook render. The constructor of this class  must be used after modification of pagesetup cell style
type: docs
url: /net/aspose.cells.rendering/workbookrender/
---
## WorkbookRender class

Represents a Workbook render. The constructor of this class , must be used after modification of pagesetup, cell style.

```csharp
public class WorkbookRender
```

## Constructors

| Name | Description |
| --- | --- |
| [WorkbookRender](workbookrender/)(Workbook, ImageOrPrintOptions) | The construct of WorkbookRender |

## Properties

| Name | Description |
| --- | --- |
| [PageCount](../../aspose.cells.rendering/workbookrender/pagecount/) { get; } | Gets the total page count of workbook. |

## Methods

| Name | Description |
| --- | --- |
| [CustomPrint](../../aspose.cells.rendering/workbookrender/customprint/)(bool, PrintPageEventArgs) | Client can control page setting of printer when print each page using this function. |
| [Dispose](../../aspose.cells.rendering/workbookrender/dispose/)() | Releases resources created and used for rendering. |
| [GetPageSizeInch](../../aspose.cells.rendering/workbookrender/getpagesizeinch/)(int) | Get page size in inch of output image. |
| [ToImage](../../aspose.cells.rendering/workbookrender/toimage/#toimage)(int) | Render certain page to a Bitmap object. |
| [ToImage](../../aspose.cells.rendering/workbookrender/toimage/#toimage_3)(Stream) | Render whole workbook as Tiff Image to stream. |
| [ToImage](../../aspose.cells.rendering/workbookrender/toimage/#toimage_4)(string) | Render whole workbook as Tiff Image to a file. |
| [ToImage](../../aspose.cells.rendering/workbookrender/toimage/#toimage_1)(int, Stream) | Render certain page to a stream. |
| [ToImage](../../aspose.cells.rendering/workbookrender/toimage/#toimage_2)(int, string) | Render certain page to a file. |
| [ToPrinter](../../aspose.cells.rendering/workbookrender/toprinter/#toprinter)(PrinterSettings) | Render workbook to Printer |
| [ToPrinter](../../aspose.cells.rendering/workbookrender/toprinter/#toprinter_2)(string) | Render workbook to Printer |
| [ToPrinter](../../aspose.cells.rendering/workbookrender/toprinter/#toprinter_1)(PrinterSettings, string) | Render workbook to Printer |
| [ToPrinter](../../aspose.cells.rendering/workbookrender/toprinter/#toprinter_4)(string, string) | Render workbook to Printer |
| [ToPrinter](../../aspose.cells.rendering/workbookrender/toprinter/#toprinter_3)(string, int, int) | (**Obsolete.**) Render workbook to Printer |

### Examples

```csharp
// Called: WorkbookRender wr = new WorkbookRender(wb, imgOpt);
[Test]
        public void Type_WorkbookRender() 
        {
            ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();
            imgOpt.PrintingPage = PrintingPageType.IgnoreBlank;

            {
                Workbook wb = new Workbook(Constants.sourcePath + "CELLSJAVA-45252/log_scale_test_1-_crashes_system.xlsx");
                WorkbookRender wr = new WorkbookRender(wb, imgOpt);
                Assert.AreEqual(4, wr.PageCount);
            }

            {
                Workbook wb = new Workbook(Constants.sourcePath + "CELLSJAVA-45252/Chart.xlsx");
                WorkbookRender wr = new WorkbookRender(wb, imgOpt);
                Assert.AreEqual(2, wr.PageCount);
            }

            {
                Workbook wb = new Workbook(Constants.sourcePath + "CELLSJAVA-45252/Calibri2.xlsx");
                WorkbookRender wr = new WorkbookRender(wb, imgOpt);
                Assert.AreEqual(3, wr.PageCount);
            }
        }
```

### See Also

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


