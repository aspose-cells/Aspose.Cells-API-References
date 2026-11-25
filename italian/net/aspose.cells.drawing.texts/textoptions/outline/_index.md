---
title: "TextOptions.Outline"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "TextOptions property. Rappresenta il formato del contorno del testo"
type: docs
url: /it/net/aspose.cells.drawing.texts/textoptions/outline/
---
## TextOptions.Outline property

Rappresenta il formato del contorno del testo.

```csharp
public LineFormat Outline { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextOptionsPropertyOutlineDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma con testo.
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 200, 100);
            shape.Text = "Sample Text";

            // Accedi alle opzioni di testo
            TextOptions textOptions = shape.TextOptions;

            // Configura le proprietà del contorno
            LineFormat outline = textOptions.Outline;
            outline.Weight = 2.48; // Set outline weight
            outline.DashStyle = MsoLineDashStyle.Solid; // Set line style
            outline.CompoundType = MsoLineStyle.Single; // Set compound type

            // Salva la cartella di lavoro
            workbook.Save("TextOutlineDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [LineFormat](../../../aspose.cells.drawing/lineformat/)
* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


