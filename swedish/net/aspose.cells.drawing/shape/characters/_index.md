---
title: "Shape.Characters"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-metod. Returnerar ett Characters-objekt som representerar ett intervall av tecken i texten"
type: docs
url: /sv/net/aspose.cells.drawing/shape/characters/
---
## Shape.Characters method

Returnerar ett Characters-objekt som representerar ett intervall av tecken i texten.

```csharp
public FontSetting Characters(int startIndex, int length)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startIndex | Int32 | Indexet för början av tecknet. |
| length | Int32 | Antalet tecken. |

### Returvärde

Characters-objekt.

### Anmärkningar

Denna metod fungerar endast på en form med titel.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodCharactersWithInt32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form med text
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);
            shape.Text = "Sample Text";

            // Hämta tecken från index 0 med längd 4
            FontSetting fontSetting = shape.Characters(0, 4);
            
            // Modifiera teckensnittinställningarna
            fontSetting.Font.Color = System.Drawing.Color.Red;
            fontSetting.Font.Size = 14;
            fontSetting.Font.IsBold = true;

            // Spara arbetsboken
            workbook.Save("ShapeCharactersDemo.xlsx");
        }
    }
}
```

### Se även

* class [FontSetting](../../../aspose.cells/fontsetting/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


