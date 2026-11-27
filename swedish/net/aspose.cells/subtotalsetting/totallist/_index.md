---
title: "SubtotalSetting.TotalList"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SubtotalSetting-egenskap. En array av nollbaserade fältförskjutningar som anger vilka fält som subtotalerna läggs till"
type: docs
url: /sv/net/aspose.cells/subtotalsetting/totallist/
---
## SubtotalSetting.TotalList property

En array av nollbaserade fältavstånd, som anger vilka fält som delsummeringar läggs till.

```csharp
public int[] TotalList { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SubtotalSettingPropertyTotalListDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Exempel på datauppsättning
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["A5"].PutValue("B");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);

            // Skapa och applicera subtotal
            CellArea area = CellArea.CreateCellArea("A1", "B5");
            worksheet.Cells.Subtotal(area, 0, ConsolidationFunction.Sum, new int[] { 1 }, true, true, true);

            // Hämta subtotalinställning för att demonstrera användning av TotalList
            SubtotalSetting subtotal = worksheet.Cells.RetrieveSubtotalSetting(area);
            Console.WriteLine("TotalList contains column index: " + subtotal.TotalList[0]);
            
            // Spara arbetsboken
            workbook.Save("SubtotalDemo.xlsx");
        }
    }
}
```

### Se även

* class [SubtotalSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


