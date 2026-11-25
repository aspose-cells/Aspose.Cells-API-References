---
title: "ScrollBar.Min"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ScrollBar. Ottiene o imposta il valore minimo di un intervallo di barra di scorrimento o spinner"
type: docs
url: /it/net/aspose.cells.drawing/scrollbar/min/
---
## ScrollBar.Min property

Ottiene o imposta il valore minimo dell'intervallo di una barra di scorrimento o di uno spinner.

```csharp
public int Min { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ScrollBarPropertyMinDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una barra di scorrimento al foglio di lavoro
            Aspose.Cells.Drawing.ScrollBar scrollBar = (Aspose.Cells.Drawing.ScrollBar)worksheet.Shapes.AddScrollBar(1, 0, 1, 1, 100, 20);

            // Imposta le proprietà della barra di scorrimento
            scrollBar.Min = 10;
            scrollBar.Max = 100;
            scrollBar.CurrentValue = 50;  // Changed from Value to CurrentValue
            scrollBar.IncrementalChange = 5;
            scrollBar.PageChange = 20;

            // Visualizza il valore della proprietà Min
            Console.WriteLine("ScrollBar Min Value: " + scrollBar.Min);

            // Salva la cartella di lavoro
            workbook.Save("ScrollBarMinDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ScrollBar](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


