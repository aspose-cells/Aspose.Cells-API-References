---
title: Class LowCodeImageSaveOptions
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.LowCode.LowCodeImageSaveOptions class. Options for saving image in low code way
type: docs
url: /net/aspose.cells.lowcode/lowcodeimagesaveoptions/
---
## LowCodeImageSaveOptions class

Options for saving image in low code way.

```csharp
public class LowCodeImageSaveOptions : LowCodeSaveOptions
```

## Constructors

| Name | Description |
| --- | --- |
| [LowCodeImageSaveOptions](lowcodeimagesaveoptions/)() | The default constructor. |

## Properties

| Name | Description |
| --- | --- |
| [ImageOptions](../../aspose.cells.lowcode/lowcodeimagesaveoptions/imageoptions/) { get; set; } | The options for rendering images. |
| [OutputFile](../../aspose.cells.lowcode/lowcodesaveoptions/outputfile/) { get; set; } | Gets and sets the file(with path if needed) for saving the generated data. When setting this property with value other than null or empty string, [`OutputStream`](../lowcodesaveoptions/outputstream/) will be ignored.(Inherited from [`LowCodeSaveOptions`](../lowcodesaveoptions/).) |
| [OutputStream](../../aspose.cells.lowcode/lowcodesaveoptions/outputstream/) { get; set; } | Gets and sets the Stream for writing the generated data to. When setting this property with value other than null, [`OutputFile`](../lowcodesaveoptions/outputfile/) will be ignored.(Inherited from [`LowCodeSaveOptions`](../lowcodesaveoptions/).) |
| override [SaveFormat](../../aspose.cells.lowcode/lowcodeimagesaveoptions/saveformat/) { get; set; } | Gets or sets the save format. |
| [SaveOptionsProvider](../../aspose.cells.lowcode/lowcodeimagesaveoptions/saveoptionsprovider/) { get; set; } | Provider of save options for saving generated images. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Rendering;
    using System;

    public class LowCodeClassLowCodeImageSaveOptionsDemo
    {
        public static void Run()
        {
            // Create a new workbook and populate with sample data
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add sample content to worksheet
            worksheet.Cells["A1"].PutValue("Sales Report");
            worksheet.Cells["A3"].PutValue("Product");
            worksheet.Cells["B3"].PutValue("Qty");
            worksheet.Cells["A4"].PutValue("Widget");
            worksheet.Cells["B4"].PutValue(150);
            worksheet.Cells["A5"].PutValue("Gadget");
            worksheet.Cells["B5"].PutValue(200);

            // Create a column chart
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B4:B5", true);
            chart.NSeries.CategoryData = "A4:A5";

            // Configure image save options
            ImageSaveOptions saveOptions = new ImageSaveOptions(SaveFormat.Png);
            saveOptions.ImageOrPrintOptions.HorizontalResolution = 300;
            saveOptions.ImageOrPrintOptions.VerticalResolution = 300;
            saveOptions.ImageOrPrintOptions.ImageType = ImageType.Png;

            // Save each worksheet as high-resolution PNG image
            workbook.Save("LowCodeImageExport.png", saveOptions);
        }
    }
}
```

### See Also

* class [LowCodeSaveOptions](../lowcodesaveoptions/)
* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


