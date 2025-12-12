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
    bool fontBold, bool fontItalic, int topRow, int top, int leftColumn, int left, int height, 
    int width)
```

| Parameter | Type | Description |
| --- | --- | --- |
| effect | MsoPresetTextEffect | The mso preset text effect type. |
| text | String | The WordArt text. |
| fontName | String | The font name. |
| size | Int32 | The font size |
| fontBold | Boolean | Indicates whether font is bold. |
| fontItalic | Boolean | Indicates whether font is italic. |
| topRow | Int32 | Upper left row index. |
| top | Int32 | Represents the vertical offset of shape from its left row, in unit of pixel. |
| leftColumn | Int32 | Upper left column index. |
| left | Int32 | Represents the horizontal offset of shape from its left column, in unit of pixel. |
| height | Int32 | Represents the height of shape, in unit of pixel. |
| width | Int32 | Represents the width of shape, in unit of pixel. |

### Return Value

Returns a Shape object that represents the new WordArt object.

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddTextEffectWithMsoPresetTextEffectStringStrinDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            Shape wordArt = shapes.AddTextEffect(
                MsoPresetTextEffect.TextEffect10,
                "Sample WordArt",
                "Arial",
                18,
                false,
                false,
                3,
                0,
                3,
                0,
                200,
                50
            );

            workbook.Save("WordArtDemo.xlsx");
        }
    }
}
```

### See Also

* class [Shape](../../shape/)
* enum [MsoPresetTextEffect](../../msopresettexteffect/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


