---
title: "ShapeCollection.AddWordArt"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeCollection-metod. Lägger till förinställd WordArt sedan Excel 2007."
type: docs
url: /sv/net/aspose.cells.drawing/shapecollection/addwordart/
---
## ShapeCollection.AddWordArt method

Lägger till förinställd WordArt sedan Excel 2007.

```csharp
public Shape AddWordArt(PresetWordArtStyle style, string text, int topRow, int top, int leftColumn, 
    int left, int height, int width)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| style | PresetWordArtStyle | Den förinställda WordArt-stilen. |
| text | String | Texten. |
| topRow | Int32 | Övre vänstra radindex. |
| top | Int32 | Representerar det vertikala offsetet för formen från dess vänstra rad, i enhet pixel. |
| leftColumn | Int32 | Övre vänstra kolumnindex. |
| vänster | Int32 | Representerar den horisontella förskjutningen av formen från dess vänstra kolumn, i enheten pixel. |
| höjd | Int32 | Representerar formens höjd, i enheten pixlar. |
| bredd | Int32 | Representerar formens bredd, i enheten pixel. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddWordArtWithPresetWordArtStyleStringInt32IDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Hämta samlingen av former
            ShapeCollection shapes = worksheet.Shapes;

            // Lägg till en WordArt med angivna parametrar
            Shape wordArt = shapes.AddWordArt(
                PresetWordArtStyle.WordArtStyle1, 
                "Sample WordArt", 
                10,  // left
                10,  // top
                200, // width
                50,  // height
                100, // rotation
                200  // z-order
            );

            // Spara arbetsboken
            workbook.Save("WordArtDemo.xlsx");
        }
    }
}
```

### Se även

* class [Shape](../../shape/)
* enum [PresetWordArtStyle](../../presetwordartstyle/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


