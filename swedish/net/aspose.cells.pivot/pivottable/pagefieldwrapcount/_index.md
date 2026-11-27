---
title: "PivotTable.PageFieldWrapCount"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable egenskap. Hämtar antalet sidfält i varje kolumn eller rad i PivotTable-rapporten"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/pagefieldwrapcount/
---
## PivotTable.PageFieldWrapCount property

Hämtar antalet sidfält i varje kolumn eller rad i PivotTable‑rapporten.

```csharp
public int PageFieldWrapCount { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyPageFieldWrapCountDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Mata in data
            Worksheet data = workbook.Worksheets.Add("data");
            data.Cells["A1"].PutValue("Country");
            data.Cells["B1"].PutValue("Product");
            data.Cells["C1"].PutValue("Vendor");
            data.Cells["D1"].PutValue("Value");
            data.Cells["A2"].PutValue("USA");
            data.Cells["B2"].PutValue("Car");
            data.Cells["C2"].PutValue("Ford");
            data.Cells["D2"].PutValue(1200.987654321);
            data.Cells["A3"].PutValue("Japan");
            data.Cells["B3"].PutValue("Bike");
            data.Cells["C3"].PutValue("Yamaha");
            data.Cells["D3"].PutValue(985.123456789);

            // Skapa pivottabell
            Worksheet pivot = workbook.Worksheets.Add("pivot");
            PivotTableCollection pivotTables = pivot.PivotTables;
            int index = pivotTables.Add("=data!A1:D3", "A1", "pivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // Lägg till fält i pivottabell
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Country");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Page, "Vendor");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");

            // Ställ in PageFieldWrapCount-egenskapen
            pivotTable.PageFieldWrapCount = 2; // Number of page fields per row
            
            // Beräkna och uppdatera pivottabell
            pivotTable.CalculateData();
            
            // Spara arbetsboken
            workbook.Save("PivotTablePageFieldWrapCountDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


