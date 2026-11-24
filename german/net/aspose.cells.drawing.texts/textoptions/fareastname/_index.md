---
title: "TextOptions.FarEastName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextOptions-Eigenschaft. Liest und setzt den FarEast-Namen"
type: docs
url: /de/net/aspose.cells.drawing.texts/textoptions/fareastname/
---
## TextOptions.FarEastName property

Liest und setzt den FarEast-Namen.

```csharp
public string FarEastName { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine Form hinzu und setze die FarEastName-Schriftart
            Aspose.Cells.Drawing.Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
            shape.Text = "Sample Text";
            shape.TextOptions.FarEastName = "宋体";

            // Speichern und neu laden, um zu überprüfen
            string outputPath = "output_FarEastName.xlsx";
            workbook.Save(outputPath);

            // Neu laden, um zu überprüfen
            Workbook verifyWorkbook = new Workbook(outputPath);
            Aspose.Cells.Drawing.Shape verifyShape = verifyWorkbook.Worksheets[0].Shapes[0];
            Console.WriteLine("FarEastName: " + verifyShape.TextOptions.FarEastName);
        }
    }
}
```

### Siehe auch

* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


