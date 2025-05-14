---
title: SheetRender.GetPageSizeInch
second_title: Aspose.Cells for .NET API Reference
description: SheetRender method. Get page size in inch of output image
type: docs
url: /net/aspose.cells.rendering/sheetrender/getpagesizeinch/
---
## SheetRender.GetPageSizeInch method

Get page size in inch of output image.

```csharp
public float[] GetPageSizeInch(int pageIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | Int32 | The page index is based on zero. |

### Return Value

Page size of image, [0] for width and [1] for height

### Examples

```csharp
// Called: var size = sheetRender.GetPageSizeInch(0);
private byte[] SheetRender_Method_GetPageSizeInch(Worksheet worksheet, string cellAddressUpperLeft, string cellAddressLowerRight)
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

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


