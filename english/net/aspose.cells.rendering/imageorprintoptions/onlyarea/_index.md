---
title: ImageOrPrintOptions.OnlyArea
second_title: Aspose.Cells for .NET API Reference
description: ImageOrPrintOptions property. If this property is true  one Area will be output and no scale will take effect
type: docs
url: /net/aspose.cells.rendering/imageorprintoptions/onlyarea/
---
## ImageOrPrintOptions.OnlyArea property

If this property is true , one Area will be output, and no scale will take effect.

```csharp
public bool OnlyArea { get; set; }
```

### Examples

```csharp
// Called: options.OnlyArea = true;
private void Property_OnlyArea(object o)
        {
            Worksheet worksheet = (Worksheet)o;
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            options.OnlyArea = true;
            SheetRender sr = new SheetRender(worksheet, options);
            using (var msImg = new MemoryStream())
            {
                Console.WriteLine(worksheet.Name + ".ToImage()...");
                sr.ToImage(0, msImg);
            }
        }
```

### See Also

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


