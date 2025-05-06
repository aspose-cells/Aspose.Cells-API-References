---
title: ImageOrPrintOptions.SmoothingMode
second_title: Aspose.Cells for .NET API Reference
description: ImageOrPrintOptions property. Specifies whether smoothing antialiasing is applied to lines and curves and the edges of filled areas. The default value is SmoothingMode.None
type: docs
url: /net/aspose.cells.rendering/imageorprintoptions/smoothingmode/
---
## ImageOrPrintOptions.SmoothingMode property

Specifies whether smoothing (antialiasing) is applied to lines and curves and the edges of filled areas. The default value is SmoothingMode.None

```csharp
public SmoothingMode SmoothingMode { get; set; }
```

### Examples

```csharp
// Called: SmoothingMode = System.Drawing.Drawing2D.SmoothingMode.HighQuality
[Test]
        public void Property_SmoothingMode()
        {
            ImageOrPrintOptions opt = new ImageOrPrintOptions()
            {
                ImageType = ImageType.Png,
#if !NETCOREAPP3_1_OR_GREATER
                SmoothingMode = System.Drawing.Drawing2D.SmoothingMode.HighQuality
#endif
            };
        }
```

### See Also

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


