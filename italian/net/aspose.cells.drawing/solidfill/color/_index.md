---
title: "SolidFill.Color"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SolidFill. Ottiene o imposta il colore."
type: docs
url: /it/net/aspose.cells.drawing/solidfill/color/
---
## SolidFill.Color property

Ottiene o imposta il colore.

```csharp
public Color Color { get; set; }
```

### Esempi

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SolidFillPropertyColorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi una forma al foglio di lavoro con i parametri corretti.
            Shape shape = sheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 100);

            // Imposta le proprietà della forma con colore.
            Color fillColor = Color.LightBlue;
            Color textColor = Color.DarkBlue;
            string text = "Solid Fill Demo";

            // Dimostra l'uso della proprietà Color.
            shape.Fill.SolidFill.Color = fillColor;
            shape.LineFormat.ForeColor = fillColor;
            shape.Text = text;
            shape.Font.Color = textColor;

            // Salva la cartella di lavoro
            workbook.Save("SolidFillPropertyColorDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SolidFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


