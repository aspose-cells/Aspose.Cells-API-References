---
title: "ScrollBar.IsHorizontal"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ScrollBar. Indica se si tratta di una barra di scorrimento orizzontale"
type: docs
url: /it/net/aspose.cells.drawing/scrollbar/ishorizontal/
---
## ScrollBar.IsHorizontal property

Indica se questa è una barra di scorrimento orizzontale.

```csharp
public bool IsHorizontal { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ScrollBarPropertyIsHorizontalDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una barra di scorrimento orizzontale
            Shape scrollBarShape = worksheet.Shapes.AddScrollBar(1, 0, 1, 0, 100, 20);
            ScrollBar scrollBar = (ScrollBar)scrollBarShape;
            scrollBar.IsHorizontal = true;

            // Aggiungi una barra di scorrimento verticale per confronto
            Shape verticalScrollBarShape = worksheet.Shapes.AddScrollBar(1, 0, 1, 30, 20, 100);
            ScrollBar verticalScrollBar = (ScrollBar)verticalScrollBarShape;
            verticalScrollBar.IsHorizontal = false;

            // Dimostra la proprietà IsHorizontal
            Console.WriteLine("Horizontal Scroll Bar IsHorizontal: " + scrollBar.IsHorizontal);
            Console.WriteLine("Vertical Scroll Bar IsHorizontal: " + verticalScrollBar.IsHorizontal);

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


