---
title: "PivotTable.CalculateRange"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-metod. Beräknar pivottabellens område"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/calculaterange/
---
## PivotTable.CalculateRange method

Beräknar pivottabellens område.

```csharp
public void CalculateRange()
```

### Anmärkningar

Om den här metoden inte har anropats, kanske pivottabellens område inte är korrekt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodCalculateRangeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till exempeldata i det första kalkylbladet
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Cells["A1"].PutValue("Product");
            dataSheet.Cells["B1"].PutValue("Sales");
            dataSheet.Cells["A2"].PutValue("Apple");
            dataSheet.Cells["B2"].PutValue(1000);
            dataSheet.Cells["A3"].PutValue("Banana");
            dataSheet.Cells["B3"].PutValue(2000);
            dataSheet.Cells["A4"].PutValue("Orange");
            dataSheet.Cells["B4"].PutValue(3000);

            // Lägg till en pivottabell
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
            int pivotIndex = pivotSheet.PivotTables.Add("A1", "A1:B4", "PivotTable1");
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
            
            // Lägg till rad- och datafält
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Beräkna område och uppdatera data
            pivotTable.CalculateRange();
            pivotTable.CalculateData();
            pivotTable.RefreshData();
            
            // Spara arbetsboken
            workbook.Save("PivotTableCalculateRangeDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


