---
title: ShapeCollection.AddTextEffect
second_title: Aspose.Cells for .NET API Reference
description: ShapeCollection method. Inserts a WordArt object
type: docs
url: /net/aspose.cells.drawing/shapecollection/addtexteffect/
---
## ShapeCollection.AddTextEffect method

Inserts a WordArt object.

```csharp
public Shape AddTextEffect(MsoPresetTextEffect effect, string text, string fontName, int size, 
    bool fontBold, bool fontItalic, int upperLeftRow, int top, int upperLeftColumn, int left, 
    int height, int width)
```

| Parameter | Type | Description |
| --- | --- | --- |
| effect | MsoPresetTextEffect | The mso preset text effect type. |
| text | String | The WordArt text. |
| fontName | String | The font name. |
| size | Int32 | The font size |
| fontBold | Boolean | Indicates whether font is bold. |
| fontItalic | Boolean | Indicates whether font is italic. |
| upperLeftRow | Int32 | Upper left row index. |
| top | Int32 | Represents the vertical offset of shape from its left row, in unit of pixel. |
| upperLeftColumn | Int32 | Upper left column index. |
| left | Int32 | Represents the horizontal offset of shape from its left column, in unit of pixel. |
| height | Int32 | Represents the height of shape, in unit of pixel. |
| width | Int32 | Represents the width of shape, in unit of pixel. |

### Return Value

Returns a Shape object that represents the new WordArt object.

### Examples

```csharp

[C#]
//add a WordArt
Shape wordArt1 = shapes.AddTextEffect(MsoPresetTextEffect.TextEffect10, "WordArt", "arial", 18, false, false, 3, 0, 3, 0, 200, 50);
```

### See Also

* class [Shape](../../shape/)
* enum [MsoPresetTextEffect](../../msopresettexteffect/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


