---
title: "Worksheet.Outline"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-egenskap. Hämtar konturen på detta kalkylblad"
type: docs
url: /sv/net/aspose.cells/worksheet/outline/
---
## Worksheet.Outline property

Hämtar konturen på detta arbetsblad.

```csharp
public Outline Outline { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyOutlineDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata och skapa konturgrupper
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[$"A{i + 1}"].Value = $"Item {i + 1}";
                worksheet.Cells[$"B{i + 1}"].Value = (i + 1) * 100;
            }

            // Gruppera rader (skapar kontur)
            worksheet.Cells.GroupRows(0, 9, false);

            // Åtkomst till konturegenskaper
            Outline outline = worksheet.Outline;
            Console.WriteLine($"Outline summary row is below detail: {outline.SummaryRowBelow}");
            Console.WriteLine($"Outline summary column is to right: {outline.SummaryColumnRight}");

            // Ändra konturinställningar
            outline.SummaryRowBelow = true;
            outline.SummaryColumnRight = false;

            // Avgruppera rader för att demonstrera konturfunktionalitet
            worksheet.Cells.UngroupRows(0, 9);

            // Spara arbetsboken
            workbook.Save("WorksheetOutlineDemo.xlsx");
        }
    }
}
```

### Se även

* class [Outline](../../outline/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


