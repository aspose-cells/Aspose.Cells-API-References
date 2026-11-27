---
title: "SubtotalSetting.SummaryBelowData"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SubtotalSetting property. Anger om en sammanfattning ska läggas till under data"
type: docs
url: /sv/net/aspose.cells/subtotalsetting/summarybelowdata/
---
## SubtotalSetting.SummaryBelowData property

Anger om en sammanfattning ska läggas till under data.

```csharp
public bool SummaryBelowData { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SubtotalSettingPropertySummaryBelowDataDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("A");
            worksheet.Cells["A4"].PutValue("B");
            worksheet.Cells["A5"].PutValue("B");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);

            // Skapa cellområde för delsummeringar
            CellArea area = CellArea.CreateCellArea("A1", "B5");

            // Applicera delsummeringar med Cells.Subtotal‑metoden med alla nödvändiga parametrar
            worksheet.Cells.Subtotal(
                area, 
                0, 
                ConsolidationFunction.Sum, 
                new int[] { 1 }, 
                false, 
                false, 
                false);  // summaryBelowData parameter

            // Hämta inställningen för att kontrollera SummaryBelowData
            SubtotalSetting retrievedSetting = worksheet.Cells.RetrieveSubtotalSetting(area);
            
            // Skriv ut värdet för egenskapen SummaryBelowData
            Console.WriteLine("SummaryBelowData: " + retrievedSetting.SummaryBelowData);
        }
    }
}
```

### Se även

* class [SubtotalSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


