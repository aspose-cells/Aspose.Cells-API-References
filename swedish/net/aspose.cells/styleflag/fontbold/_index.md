---
title: "StyleFlag.FontBold"
second_title: "Aspose.Cells för .NET API‑referens"
description: "StyleFlag egenskap. Inställning för fet font kommer att tillämpas"
type: docs
url: /sv/net/aspose.cells/styleflag/fontbold/
---
## StyleFlag.FontBold property

Inställning för fetstil i teckensnittet kommer att tillämpas.

```csharp
public bool FontBold { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyFontBoldDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en fet stil
            Style boldStyle = workbook.CreateStyle();
            boldStyle.Font.IsBold = true;

            // Applicera fet stil på rad 2 med StyleFlag för endast FontBold
            worksheet.Cells.ApplyRowStyle(1, boldStyle, new StyleFlag { FontBold = true });

            // Sätt värde i cellen för att demonstrera stilen
            worksheet.Cells[1, 0].PutValue("Bold Text");

            // Spara arbetsboken
            workbook.Save("output.xlsx");

            Console.WriteLine("FontBold property demo completed successfully.");
        }
    }
}
```

### Se även

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


