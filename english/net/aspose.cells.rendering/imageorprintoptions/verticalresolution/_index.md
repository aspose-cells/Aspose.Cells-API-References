---
title: ImageOrPrintOptions.VerticalResolution
second_title: Aspose.Cells for .NET API Reference
description: ImageOrPrintOptions property. Gets or sets the vertical resolution for generated images in dots per inch
type: docs
url: /net/aspose.cells.rendering/imageorprintoptions/verticalresolution/
---
## ImageOrPrintOptions.VerticalResolution property

Gets or sets the vertical resolution for generated images, in dots per inch.

```csharp
public int VerticalResolution { get; set; }
```

### Remarks

The default value is 96.

Setting [`HorizontalResolution`](../horizontalresolution/) and `VerticalResolution` effects the width and height of the output image in pixels.

### Examples

The following code sets resolution to 192, the width and height of the generated image is twice of the one with resolution left as the default value 96.

```csharp
Workbook wb = new Workbook("Book1.xlsx");

ImageOrPrintOptions opts = new ImageOrPrintOptions();

//Set output image type: png.
opts.ImageType = ImageType.Png;

//Set resolution to 192.
opts.HorizontalResolution = 192;
opts.VerticalResolution = 192;

//Render Chart to image.
wb.Worksheets[0].Charts[0].ToImage("Chart.png", opts);
```

### See Also

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


