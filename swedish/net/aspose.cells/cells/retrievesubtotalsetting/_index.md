---
title: "Cells.RetrieveSubtotalSetting"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Hämtar subtotalinställning för området"
type: docs
url: /sv/net/aspose.cells/cells/retrievesubtotalsetting/
---
## Cells.RetrieveSubtotalSetting method

Hämtar subtotalinställningarna för området.

```csharp
public SubtotalSetting RetrieveSubtotalSetting(CellArea ca)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ca | CellArea | Området |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodRetrieveSubtotalSettingWithCellAreaDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för subtotaler
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells["A" + i].PutValue(i % 2 == 0 ? "Group1" : "Group2");
                worksheet.Cells["B" + i].PutValue(i * 100);
            }

            // Skapa subtotaler
            CellArea area = CellArea.CreateCellArea("A1", "B10");
            worksheet.Cells.Subtotal(area, 0, ConsolidationFunction.Sum, new int[] { 1 });

            // Hämta subtotalinställningar
            SubtotalSetting setting = worksheet.Cells.RetrieveSubtotalSetting(area);

            // Utskriftsinställningar
            Console.WriteLine("GroupBy: " + setting.GroupBy);
            Console.WriteLine("Function: " + setting.SubtotalFunction);
            Console.WriteLine("SummaryBelowData: " + setting.SummaryBelowData);
            Console.WriteLine("TotalList: " + string.Join(",", setting.TotalList));
        }
    }
}
```

### Se även

* class [SubtotalSetting](../../subtotalsetting/)
* struct [CellArea](../../cellarea/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


