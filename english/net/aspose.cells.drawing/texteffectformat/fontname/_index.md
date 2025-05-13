---
title: TextEffectFormat.FontName
second_title: Aspose.Cells for .NET API Reference
description: TextEffectFormat property. The name of the font used in the WordArt
type: docs
url: /net/aspose.cells.drawing/texteffectformat/fontname/
---
## TextEffectFormat.FontName property

The name of the font used in the WordArt.

```csharp
public string FontName { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual("+mn-ea", shape.TextEffect.FontName);
public void TextEffectFormat_Property_FontName()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
    Shape shape = workbook.Worksheets[0].Shapes[1];
    Assert.AreEqual("+mn-ea", shape.TextEffect.FontName);
}
```

### See Also

* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


