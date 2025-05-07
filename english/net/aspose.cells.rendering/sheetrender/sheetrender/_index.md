---
title: SheetRender.SheetRender
second_title: Aspose.Cells for .NET API Reference
description: SheetRender constructor. the construct of SheetRender need worksheet and ImageOrPrintOptions as params
type: docs
url: /net/aspose.cells.rendering/sheetrender/sheetrender/
---
## SheetRender constructor

the construct of SheetRender, need worksheet and ImageOrPrintOptions as params

```csharp
public SheetRender(Worksheet worksheet, ImageOrPrintOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| worksheet | Worksheet | Indicate which spreadsheet to be rendered. |
| options | ImageOrPrintOptions | ImageOrPrintOptions contains some property of output image |

### Examples

```csharp
// Called: var sheetRender = new SheetRender(worksheet, options);
private byte[] SheetRender_Constructor(Worksheet worksheet, string cellAddressUpperLeft, string cellAddressLowerRight)
        {
            // Set the print area range
            worksheet.PageSetup.PrintArea = cellAddressUpperLeft + ":" + cellAddressLowerRight;
            // Set all margins to zero
            worksheet.PageSetup.LeftMargin = 0;
            worksheet.PageSetup.RightMargin = 0;
            worksheet.PageSetup.TopMargin = 0;
            worksheet.PageSetup.BottomMargin = 0;
            // Create image options
            var options = new ImageOrPrintOptions
            {
                OnePagePerSheet = true,
                ImageType = ImageType.Png,
                //SaveFormat = Aspose.Cells.SaveFormat.Svg,
                HorizontalResolution = 200,
                VerticalResolution = 200
            };
            // Create image of the worksheet
            var sheetRender = new SheetRender(worksheet, options);
            MemoryStream rangeStream = new MemoryStream();
            sheetRender.ToImage(0, rangeStream);
            var size = sheetRender.GetPageSizeInch(0);
            var bytes = rangeStream.ToArray();
            return bytes;
        }
```

### See Also

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [ImageOrPrintOptions](../../imageorprintoptions/)
* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


