---
title: "TextOptions.FarEastName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextOptions egenskap. Hämtar och anger FarEast-namnet"
type: docs
url: /sv/net/aspose.cells.drawing.texts/textoptions/fareastname/
---
## TextOptions.FarEastName property

Hämtar och anger FarEast-namnet.

```csharp
public string FarEastName { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextOptionsPropertyFarEastNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form och ange FarEastName-typsnitt
            Aspose.Cells.Drawing.Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
            shape.Text = "Sample Text";
            shape.TextOptions.FarEastName = "宋体";

            // Spara och ladda om för att verifiera
            string outputPath = "output_FarEastName.xlsx";
            workbook.Save(outputPath);

            // Ladda om för att verifiera
            Workbook verifyWorkbook = new Workbook(outputPath);
            Aspose.Cells.Drawing.Shape verifyShape = verifyWorkbook.Worksheets[0].Shapes[0];
            Console.WriteLine("FarEastName: " + verifyShape.TextOptions.FarEastName);
        }
    }
}
```

### Se även

* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


