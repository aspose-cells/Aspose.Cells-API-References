---
title: "Workbook.Colors"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-egenskap. Returnerar färger i paletten för kalkylbladet"
type: docs
url: /sv/net/aspose.cells/workbook/colors/
---
## Workbook.Colors property

Returnerar färger i paletten för kalkylbladet.

```csharp
public Color[] Colors { get; }
```

### Anmärkningar

Paletten har 56 poster, var och en representerad av ett RGB‑värde.

### Exempel

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyColorsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Kom åt standardfärgpaletten
            Color[] colors = workbook.Colors;

            // Ändra några färger i paletten
            colors[0] = System.Drawing.Color.Red;      // Modify first color to Red
            colors[1] = System.Drawing.Color.Green;    // Modify second color to Green
            colors[2] = System.Drawing.Color.Blue;    // Modify third color to Blue

            // Skapa ett arbetsblad och lägg till lite data
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Color Demo");
            
            // Applicera de ändrade färgerna på celler
            Style style1 = workbook.CreateStyle();
            style1.ForegroundColor = colors[0];
            style1.Pattern = BackgroundType.Solid;
            worksheet.Cells["A2"].SetStyle(style1);
            
            Style style2 = workbook.CreateStyle();
            style2.ForegroundColor = colors[1];
            style2.Pattern = BackgroundType.Solid;
            worksheet.Cells["B2"].SetStyle(style2);
            
            Style style3 = workbook.CreateStyle();
            style3.ForegroundColor = colors[2];
            style3.Pattern = BackgroundType.Solid;
            worksheet.Cells["C2"].SetStyle(style3);

            // Spara arbetsboken
            workbook.Save("WorkbookColorsDemo.xlsx");
        }
    }
}
```

### Se även

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


