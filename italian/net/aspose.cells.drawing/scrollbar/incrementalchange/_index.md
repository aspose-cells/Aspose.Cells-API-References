---
title: "ScrollBar.IncrementalChange"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ScrollBar. Ottiene o imposta la quantità con cui la barra di scorrimento o lo spinner viene incrementato di una linea di scorrimento"
type: docs
url: /it/net/aspose.cells.drawing/scrollbar/incrementalchange/
---
## ScrollBar.IncrementalChange property

Ottiene o imposta la quantità di incremento della barra di scorrimento o dello spinner per una linea di scorrimento.

```csharp
public int IncrementalChange { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ScrollBarPropertyIncrementalChangeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una barra di scorrimento al foglio di lavoro
            ScrollBar scrollBar = worksheet.Shapes.AddScrollBar(1, 0, 1, 1, 100, 20);

            // Imposta le proprietà della barra di scorrimento
            scrollBar.Min = 0;
            scrollBar.Max = 100;
            scrollBar.CurrentValue = 50;
            scrollBar.IncrementalChange = 5; // This is the key property we're demonstrating
            scrollBar.PageChange = 20;

            // Visualizza le proprietà della barra di scorrimento
            Console.WriteLine("Scroll Bar Properties:");
            Console.WriteLine("Min: " + scrollBar.Min);
            Console.WriteLine("Max: " + scrollBar.Max);
            Console.WriteLine("Current Value: " + scrollBar.CurrentValue);
            Console.WriteLine("Incremental Change: " + scrollBar.IncrementalChange);
            Console.WriteLine("Page Change: " + scrollBar.PageChange);

            // Modifica la variazione incrementale
            scrollBar.IncrementalChange = 10;
            Console.WriteLine("\nModified Incremental Change: " + scrollBar.IncrementalChange);

            // Salva la cartella di lavoro
            workbook.Save("ScrollBarDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ScrollBar](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


