---
title: "TextBoxOptions.ShapeTextDirection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextBoxOptions. Ottiene o imposta la direzione di visualizzazione del testo all'interno di un determinato corpo di testo. Corrisponde a Format Shape  Text Options  Text Box  Text direction in Excel"
type: docs
url: /it/net/aspose.cells.drawing.texts/textboxoptions/shapetextdirection/
---
## TextBoxOptions.ShapeTextDirection property

Ottiene o imposta la direzione di visualizzazione del testo all'interno di un determinato corpo di testo. Corrisponde a "Format Shape - Text Options - Text Box - Text direction" in Excel

```csharp
public TextVerticalType ShapeTextDirection { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextBoxOptionsPropertyShapeTextDirectionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma di casella di testo
            Shape shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 200);

            // Imposta la direzione del testo su verticale
            shape.TextBoxOptions.ShapeTextDirection = TextVerticalType.Vertical;

            // Imposta del testo per dimostrare la direzione
            shape.Text = "Vertical Text Example";

            // Salva la cartella di lavoro
            workbook.Save("TextBoxTextDirectionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [TextVerticalType](../../textverticaltype/)
* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


