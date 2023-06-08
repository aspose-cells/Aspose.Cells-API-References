---
title: ImageOrPrintOptions.TiffColorDepth
second_title: Aspose.Cells for .NET API Reference
description: ImageOrPrintOptions property. Gets or sets bit depth to apply only when saving pages to the Tiff format
type: docs
url: /net/aspose.cells.rendering/imageorprintoptions/tiffcolordepth/
---
## ImageOrPrintOptions.TiffColorDepth property

Gets or sets bit depth to apply only when saving pages to the `Tiff` format.

```csharp
public ColorDepth TiffColorDepth { get; set; }
```

### Remarks

Has effect only when saving to TIFF. If TiffCompression is set to CCITT3, CCITT4, this will not take effect, the bit depth of the generated tiff image will be always 1.

### See Also

* enum [ColorDepth](../../colordepth/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


