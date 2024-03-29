---
title: ShapeCollection.AddWordArt
second_title: Aspose.Cells for .NET API Reference
description: ShapeCollection method. Adds preset WordArt since Excel 2007.s
type: docs
url: /net/aspose.cells.drawing/shapecollection/addwordart/
---
## ShapeCollection.AddWordArt method

Adds preset WordArt since Excel 2007.s

```csharp
public Shape AddWordArt(PresetWordArtStyle style, string text, int upperLeftRow, int top, 
    int upperLeftColumn, int left, int height, int width)
```

| Parameter | Type | Description |
| --- | --- | --- |
| style | PresetWordArtStyle | The preset WordArt Style. |
| text | String | The text. |
| upperLeftRow | Int32 | Upper left row index. |
| top | Int32 | Represents the vertical offset of shape from its left row, in unit of pixel. |
| upperLeftColumn | Int32 | Upper left column index. |
| left | Int32 | Represents the horizontal offset of shape from its left column, in unit of pixel. |
| height | Int32 | Represents the height of shape, in unit of pixel. |
| width | Int32 | Represents the width of shape, in unit of pixel. |

### Examples

```csharp

[C#]
//add a WordArt
Shape wordArt2 = shapes.AddWordArt(PresetWordArtStyle.WordArtStyle1, "WordArt", 3, 0, 3, 0, 50, 200);
```

### See Also

* class [Shape](../../shape/)
* enum [PresetWordArtStyle](../../presetwordartstyle/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


