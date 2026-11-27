---
title: "PivotTable.DisplayNullString"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-egenskap. Anger om PivotTable-rapporten visar en anpassad sträng när värdet är null"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/displaynullstring/
---
## PivotTable.DisplayNullString property

Anger om pivottabellsrapporten visar en anpassad sträng om värdet är null.

```csharp
public bool DisplayNullString { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyDisplayNullStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till ett kalkylblad och fyll i med exempeldata
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue(null);
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(null);

            // Skapa pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Konfigurera pivottabell
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Ställ in egenskapen DisplayNullString och anpassad null-sträng
            pivotTable.DisplayNullString = true;
            pivotTable.NullString = "N/A";
            
            // Beräkna data och uppdatera pivottabell
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Spara arbetsboken
            workbook.Save("PivotTableDisplayNullStringDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


