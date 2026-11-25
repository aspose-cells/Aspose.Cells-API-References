---
title: "Shape.TextHorizontalOverflow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Ottiene e imposta il tipo di overflow orizzontale del testo della forma che contiene testo"
type: docs
url: /it/net/aspose.cells.drawing/shape/texthorizontaloverflow/
---
## Shape.TextHorizontalOverflow property

Ottiene e imposta il tipo di overflow orizzontale del testo della forma che contiene testo.

```csharp
public TextOverflowType TextHorizontalOverflow { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextHorizontalOverflowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma casella di testo con i parametri corretti
            TextBox textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 200);
            textBox.Text = "This is a long text that will demonstrate text horizontal overflow functionality";

            // Imposta il tipo di overflow iniziale a Clip
            textBox.TextHorizontalOverflow = TextOverflowType.Clip;
            Console.WriteLine("TextHorizontalOverflow set to Clip (text will be clipped)");

            // Cambia il tipo di overflow a Overflow
            textBox.TextHorizontalOverflow = TextOverflowType.Overflow;
            Console.WriteLine("TextHorizontalOverflow changed to Overflow (text will overflow)");

            // Salva la cartella di lavoro
            workbook.Save("TextHorizontalOverflowDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [TextOverflowType](../../textoverflowtype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


