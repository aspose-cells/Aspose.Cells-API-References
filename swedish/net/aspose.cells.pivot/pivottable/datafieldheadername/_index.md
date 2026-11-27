---
title: "PivotTable.DataFieldHeaderName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-egenskap. Hämtar och anger namnet på värdeområdesfältets rubrik i PivotTable"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/datafieldheadername/
---
## PivotTable.DataFieldHeaderName property

Hämtar och anger namnet på fältrubriken för värdeområdet i pivottabellen.

```csharp
public string DataFieldHeaderName { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyDataFieldHeaderNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för pivottabell
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "Bike";
            cells["B2"].Value = 1000;
            cells["A3"].Value = "Car";
            cells["B3"].Value = 2000;
            cells["A4"].Value = "Bike";
            cells["B4"].Value = 1500;
            cells["A5"].Value = "Car";
            cells["B5"].Value = 3000;

            // Skapa pivottabell
            int index = sheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Konfigurera pivottabell
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Sales
            
            // Ange anpassat namn för datafältets rubrik
            pivotTable.DataFieldHeaderName = "AsposeValues";
            
            // Uppdatera och beräkna pivottabell
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Spara arbetsboken
            workbook.Save("PivotTableDataFieldHeaderNameDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


