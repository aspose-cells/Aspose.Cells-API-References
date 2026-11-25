---
title: "ScrollBar.PageChange"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ScrollBar. Ottiene o imposta la modifica della pagina"
type: docs
url: /it/net/aspose.cells.drawing/scrollbar/pagechange/
---
## ScrollBar.PageChange property

Ottiene o imposta il cambio di pagina

```csharp
public int PageChange { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ScrollBarPropertyPageChangeDemo
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
            scrollBar.IncrementalChange = 1;
            scrollBar.PageChange = 10; // Demonstrate PageChange property
            scrollBar.LinkedCell = "A1";

            // Salva la cartella di lavoro
            workbook.Save("ScrollBarPropertyPageChangeDemo.xlsx");

            // Carica la cartella di lavoro salvata per verificare le proprietà
            Workbook verifyWorkbook = new Workbook("ScrollBarPropertyPageChangeDemo.xlsx");
            ScrollBar verifyScrollBar = (ScrollBar)verifyWorkbook.Worksheets[0].Shapes[0];

            // Visualizza il valore della proprietà PageChange per dimostrare che è stato salvato/caricato correttamente
            Console.WriteLine("ScrollBar PageChange value: " + verifyScrollBar.PageChange);
        }
    }
}
```

### Vedi anche

* class [ScrollBar](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


