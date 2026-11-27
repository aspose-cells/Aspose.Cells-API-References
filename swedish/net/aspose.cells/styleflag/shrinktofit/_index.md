---
title: "StyleFlag.ShrinkToFit"
second_title: "Aspose.Cells för .NET API‑referens"
description: "StyleFlag-egenskap. Inställning för krympa för att passa kommer att tillämpas"
type: docs
url: /sv/net/aspose.cells/styleflag/shrinktofit/
---
## StyleFlag.ShrinkToFit property

Inställning för krympa för att passa kommer att tillämpas.

```csharp
public bool ShrinkToFit { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyShrinkToFitDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ange exempeldata i en cell
            cells["A1"].PutValue("This is a long text that needs to fit in the cell");
            
            // Skapa en stil med ShrinkToFit aktiverat
            Style style = workbook.CreateStyle();
            style.ShrinkToFit = true;
            
            // Skapa stilflagga och aktivera ShrinkToFit-flaggan
            StyleFlag flag = new StyleFlag();
            flag.ShrinkToFit = true;
            
            // Applicera stilen på cellintervallet (explicit med Aspose.Cells.Range)
            Aspose.Cells.Range range = cells.CreateRange("A1");
            range.ApplyStyle(style, flag);
            
            // Ställ in kolumnbredd för att demonstrera krympning
            worksheet.Cells.SetColumnWidth(0, 10);
            
            // Spara arbetsboken
            workbook.Save("ShrinkToFitDemo.xlsx");
        }
    }
}
```

### Se även

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


