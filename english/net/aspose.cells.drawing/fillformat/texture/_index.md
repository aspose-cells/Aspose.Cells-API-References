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
// Called: AssertHelper.AreEqual(TextureType.Cork, aseries.Area.FillFormat.Texture, "chart.NSeries[0].Area.FillFormat.Texture");
private void Property_Texture(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets[0];
            Chart chart = sheet.Charts[0];
            Series aseries = chart.NSeries[0];
            AssertHelper.AreEqual(TextureType.Cork, aseries.Area.FillFormat.Texture, "chart.NSeries[0].Area.FillFormat.Texture");
        }
```

### See Also

* enum [TextureType](../../texturetype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


