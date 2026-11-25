---
title: "MsoLineFormat.BackColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà MsoLineFormat. Ottiene e imposta il colore di sfondo della linea del bordo"
type: docs
url: /it/net/aspose.cells.drawing/msolineformat/backcolor/
---
## MsoLineFormat.BackColor property

Ottiene e imposta il colore di sfondo della linea del bordo.

```csharp
public Color BackColor { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoLineFormatPropertyBackColorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma linea
            Shape line = worksheet.Shapes.AddLine(1, 1, 100, 100, 5, 5);

            // Imposta le proprietà della linea
            line.LineFormat.ForeColor = Color.Red;
            line.LineFormat.BackColor = Color.Yellow; // Demonstrating BackColor usage
            line.LineFormat.DashStyle = MsoLineDashStyle.Solid;
            line.LineFormat.Weight = 2.0;

            // Salva la cartella di lavoro
            workbook.Save("LineFormatBackColorDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


