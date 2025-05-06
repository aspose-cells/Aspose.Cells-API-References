---
title: FillFormat.Texture
second_title: Aspose.Cells for .NET API Reference
description: FillFormat property. Represents the texture type for the specified fill
type: docs
url: /net/aspose.cells.drawing/fillformat/texture/
---
## FillFormat.Texture property

Represents the texture type for the specified fill.

```csharp
public TextureType Texture { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(TextureType.Granite, p.Area.FillFormat.Texture, &amp;quot;chart.NSeries[3].Area.FillFormat.Texture&amp;quot;);
private void Property_Texture(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets[&quot;Sheet2&quot;];
            Chart chart = sheet.Charts[0];
           // Series aseries = chart.NSeries[3];
            ChartPoint p = chart.NSeries[0].Points[3];
            AssertHelper.AreEqual(TextureType.Granite, p.Area.FillFormat.Texture, &quot;chart.NSeries[3].Area.FillFormat.Texture&quot;);
        }
```

### See Also

* enum [TextureType](../../texturetype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


