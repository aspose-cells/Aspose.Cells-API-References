---
title: "ShapeCollection.AddTextEffect"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeCollection-metod. Infogar ett WordArt-objekt"
type: docs
url: /sv/net/aspose.cells.drawing/shapecollection/addtexteffect/
---
## ShapeCollection.AddTextEffect method

Infogar ett WordArt-objekt.

```csharp
public Shape AddTextEffect(MsoPresetTextEffect effect, string text, string fontName, int size, 
    bool fontBold, bool fontItalic, int topRow, int top, int leftColumn, int left, int height, 
    int width)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| effekt | MsoPresetTextEffect | Typen av mso förinställd texteffekt. |
| text | String | WordArt-texten. |
| fontName | String | Typsnittets namn. |
| storlek | Int32 | Typsnittsstorleken |
| fontBold | Boolean | Anger om teckensnittet är fetstil. |
| fontItalic | Boolean | Anger om teckensnittet är kursiv. |
| topRow | Int32 | Övre vänstra radindex. |
| top | Int32 | Representerar det vertikala offsetet för formen från dess vänstra rad, i enhet pixel. |
| leftColumn | Int32 | Övre vänstra kolumnindex. |
| vänster | Int32 | Representerar den horisontella förskjutningen av formen från dess vänstra kolumn, i enheten pixel. |
| höjd | Int32 | Representerar formens höjd, i enheten pixlar. |
| bredd | Int32 | Representerar formens bredd, i enheten pixel. |

### Returvärde

Returnerar ett Shape-objekt som representerar det nya WordArt-objektet.

### Exempel

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

### Se även

* class [Shape](../../shape/)
* enum [MsoPresetTextEffect](../../msopresettexteffect/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


