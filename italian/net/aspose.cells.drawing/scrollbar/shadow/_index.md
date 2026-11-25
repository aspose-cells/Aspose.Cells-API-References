---
title: "ScrollBar.Shadow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ScrollBar. Indica se la forma ha ombreggiatura 3D"
type: docs
url: /it/net/aspose.cells.drawing/scrollbar/shadow/
---
## ScrollBar.Shadow property

Indica se la forma ha ombreggiatura 3-D.

```csharp
public bool Shadow { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ScrollBarPropertyShadowDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una barra di scorrimento orizzontale
            ScrollBar scrollBar = worksheet.Shapes.AddScrollBar(1, 0, 1, 1, 100, 20);
            
            // Imposta le proprietà della barra di scorrimento
            scrollBar.Min = 0;
            scrollBar.Max = 100;
            scrollBar.IncrementalChange = 5;
            scrollBar.PageChange = 20;
            scrollBar.CurrentValue = 50;
            scrollBar.IsHorizontal = true;
            
            // Dimostra la proprietà Shadow
            scrollBar.Shadow = true; // Enable 3D shadow effect
            
            // Crea un'altra barra di scorrimento per il confronto
            ScrollBar scrollBar2 = worksheet.Shapes.AddScrollBar(1, 2, 1, 1, 100, 20);
            scrollBar2.Shadow = false; // No shadow
            
            // Salva la cartella di lavoro
            workbook.Save("ScrollBarShadowDemo.xlsx");
            
            Console.WriteLine("ScrollBar Shadow demo completed. Check output file.");
        }
    }
}
```

### Vedi anche

* class [ScrollBar](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


