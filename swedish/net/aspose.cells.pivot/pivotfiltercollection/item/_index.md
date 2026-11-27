---
title: "PivotFilterCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotFilterCollection egenskap. Hämtar pivotfilter‑objektet på det specifika indexet"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfiltercollection/item/
---
## PivotFilterCollection indexer

Hämtar pivotfilter-objektet på det specifika indexet.

```csharp
public PivotFilter this[int index] { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för pivottabell
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 150;

            // Skapa pivottabell
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Lägg till pivotfilter med metoden PivotFilterCollection.Add
            pivotTable.PivotFilters.Add(0, PivotFilterType.Count);
            PivotFilter filter = pivotTable.PivotFilters[0]; // Using Item property via index
            filter.Name = "SampleFilter";
            filter.Value1 = "100";
            
            // Åtkomst till filter med Item‑egenskapen och visa information
            Console.WriteLine("Filter Name: " + pivotTable.PivotFilters[0].Name);
            Console.WriteLine("Filter Value1: " + pivotTable.PivotFilters[0].Value1);
            Console.WriteLine("Filter Type: " + pivotTable.PivotFilters[0].FilterType);
            
            // Spara arbetsboken
            workbook.Save("PivotFilterDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotFilter](../../pivotfilter/)
* class [PivotFilterCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


