---
title: "PivotTable.ErrorString"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable egenskap. Hämtar den sträng som visas i celler som innehåller fel när egenskapen DisplayErrorString är sann. Standardvärdet är en tom sträng"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/errorstring/
---
## PivotTable.ErrorString property

Hämtar den sträng som visas i celler som innehåller fel när egenskapen DisplayErrorString är sann. Standardvärdet är en tom sträng.

```csharp
public string ErrorString { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyErrorStringDemo
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
            cells["B5"].Value = 1800;

            // Skapa pivottabell
            int index = sheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Ange ErrorString egenskap
            pivotTable.ErrorString = "Custom Error";
            pivotTable.DisplayErrorString = true;

            // Lägg till fält i pivottabell
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Beräkna data och uppdatera pivottabell
            pivotTable.CalculateData();
            pivotTable.RefreshData();

            // Spara arbetsboken
            workbook.Save("PivotTableErrorStringDemo.xlsx");

            Console.WriteLine("PivotTable with ErrorString property set successfully.");
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


