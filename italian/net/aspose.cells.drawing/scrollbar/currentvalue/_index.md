---
title: "ScrollBar.CurrentValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ScrollBar. Ottiene o imposta il valore corrente"
type: docs
url: /it/net/aspose.cells.drawing/scrollbar/currentvalue/
---
## ScrollBar.CurrentValue property

Ottiene o imposta il valore corrente.

```csharp
public int CurrentValue { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ScrollBarPropertyCurrentValueDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una barra di scorrimento al foglio di lavoro
            Aspose.Cells.Drawing.ScrollBar scrollBar = (Aspose.Cells.Drawing.ScrollBar)worksheet.Shapes.AddScrollBar(1, 0, 1, 1, 100, 20);

            // Imposta le proprietà della barra di scorrimento usando i nomi di proprietà corretti
            scrollBar.Min = 0;
            scrollBar.Max = 100;
            scrollBar.IncrementalChange = 5;
            scrollBar.PageChange = 20;

            // Imposta e dimostra la proprietà CurrentValue
            scrollBar.CurrentValue = 50;
            Console.WriteLine("ScrollBar CurrentValue: " + scrollBar.CurrentValue);

            // Modifica il valore corrente
            scrollBar.CurrentValue = 75;
            Console.WriteLine("Updated ScrollBar CurrentValue: " + scrollBar.CurrentValue);

            // Salva la cartella di lavoro
            workbook.Save("ScrollBarCurrentValueDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ScrollBar](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


