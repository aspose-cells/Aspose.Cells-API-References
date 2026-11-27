---
title: "ScrollBar.Shadow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ScrollBar-egenskap. Anger om formen har 3D-skuggning"
type: docs
url: /sv/net/aspose.cells.drawing/scrollbar/shadow/
---
## ScrollBar.Shadow property

Anger om formen har 3‑D‑skuggning.

```csharp
public bool Shadow { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en horisontell rullningslist
            ScrollBar scrollBar = worksheet.Shapes.AddScrollBar(1, 0, 1, 1, 100, 20);
            
            // Ställ in rullningsfältsegenskaper
            scrollBar.Min = 0;
            scrollBar.Max = 100;
            scrollBar.IncrementalChange = 5;
            scrollBar.PageChange = 20;
            scrollBar.CurrentValue = 50;
            scrollBar.IsHorizontal = true;
            
            // Demonstrera Shadow-egenskapen
            scrollBar.Shadow = true; // Enable 3D shadow effect
            
            // Skapa en annan rullningslist för jämförelse
            ScrollBar scrollBar2 = worksheet.Shapes.AddScrollBar(1, 2, 1, 1, 100, 20);
            scrollBar2.Shadow = false; // No shadow
            
            // Spara arbetsboken
            workbook.Save("ScrollBarShadowDemo.xlsx");
            
            Console.WriteLine("ScrollBar Shadow demo completed. Check output file.");
        }
    }
}
```

### Se även

* class [ScrollBar](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


