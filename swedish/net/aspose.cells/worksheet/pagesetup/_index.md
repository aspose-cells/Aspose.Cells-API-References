---
title: "Worksheet.PageSetup"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-egenskap. Representerar sidinställningsbeskrivningen i detta blad"
type: docs
url: /sv/net/aspose.cells/worksheet/pagesetup/
---
## Worksheet.PageSetup property

Representerar sidinställningsbeskrivningen i detta blad.

```csharp
public PageSetup PageSetup { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyPageSetupDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ställ in sidinställningsegenskaper
            worksheet.PageSetup.PrintArea = "A1:L50";
            worksheet.PageSetup.PrintTitleRows = "1:2";
            worksheet.PageSetup.PrintTitleColumns = "A:B";
            worksheet.PageSetup.Orientation = PageOrientationType.Landscape;
            worksheet.PageSetup.PaperSize = PaperSizeType.PaperA4;
            
            // Lägg till lite exempeldata
            worksheet.Cells["A1"].PutValue("Sample Data");
            for (int i = 1; i <= 10; i++)
            {
                worksheet.Cells["A" + (i + 1)].PutValue("Item " + i);
                worksheet.Cells["B" + (i + 1)].PutValue(i * 100);
            }
            
            // Spara arbetsboken
            workbook.Save("PageSetupDemo.xlsx");
            
            Console.WriteLine("Worksheet page setup demo completed successfully.");
        }
    }
}
```

### Se även

* class [PageSetup](../../pagesetup/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


