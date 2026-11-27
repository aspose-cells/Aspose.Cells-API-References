---
title: "WorksheetCollection.ClearPivottables"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorksheetCollection-metod. Rensar pivottabeller från kalkylbladet"
type: docs
url: /sv/net/aspose.cells/worksheetcollection/clearpivottables/
---
## WorksheetCollection.ClearPivottables method

Rensar pivottabeller från kalkylbladet.

```csharp
public void ClearPivottables()
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodClearPivottablesDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa exempeldata för pivottabell
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(300);

            // Lägg till en pivottabell
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            Aspose.Cells.Pivot.PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            Console.WriteLine("Pivot tables count before clearing: " + worksheet.PivotTables.Count);

            // Rensa alla pivottabeller från alla kalkylblad
            workbook.Worksheets.ClearPivottables();

            Console.WriteLine("Pivot tables count after clearing: " + worksheet.PivotTables.Count);
        }
    }
}
```

### Se även

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


