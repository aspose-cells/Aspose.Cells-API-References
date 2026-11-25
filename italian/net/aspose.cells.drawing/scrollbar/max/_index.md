---
title: "ScrollBar.Max"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ScrollBar. Ottiene o imposta il valore massimo dell'intervallo di una barra di scorrimento o di uno spinner"
type: docs
url: /it/net/aspose.cells.drawing/scrollbar/max/
---
## ScrollBar.Max property

Ottiene o imposta il valore massimo dell'intervallo di una barra di scorrimento o di uno spinner.

```csharp
public int Max { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ScrollBarPropertyMaxDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una barra di scorrimento al foglio di lavoro
            Aspose.Cells.Drawing.ScrollBar scrollBar = (Aspose.Cells.Drawing.ScrollBar)worksheet.Shapes.AddScrollBar(1, 0, 1, 1, 100, 20);

            // Imposta le proprietà della barra di scorrimento
            scrollBar.Min = 0;
            scrollBar.Max = 100; // Demonstrating Max property usage
            scrollBar.CurrentValue = 50;
            scrollBar.IncrementalChange = 5;
            scrollBar.PageChange = 10;

            // Salva la cartella di lavoro
            workbook.Save("ScrollBarMaxDemo.xlsx");

            // Visualizza le informazioni
            Console.WriteLine("ScrollBar created with Max value: " + scrollBar.Max.ToString());
            Console.WriteLine("File saved successfully.");
        }
    }
}
```

### Vedi anche

* class [ScrollBar](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


