---
title: "PivotTable.ColumnFields"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-egenskap. Returnerar ett PivotFields-objekt som för närvarande visas som kolumnfält"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/columnfields/
---
## PivotTable.ColumnFields property

Returnerar ett PivotFields-objekt som för närvarande visas som kolumnfält.

```csharp
public PivotFieldCollection ColumnFields { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyColumnFieldsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabell
            var cells = worksheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "Bikes";
            cells["B2"].Value = 100;
            cells["A3"].Value = "Bikes";
            cells["B3"].Value = 200;
            cells["A4"].Value = "Cars";
            cells["B4"].Value = 300;
            cells["A5"].Value = "Cars";
            cells["B5"].Value = 400;
            cells["A6"].Value = "Trucks";
            cells["B6"].Value = 500;

            // Lägg till pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:B6", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Lägg till rad- och kolumnfält
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Sales");

            // Åtkomst och manipulering av kolumnfält
            PivotField columnField = pivotTable.ColumnFields[0];
            columnField.FilterByValue(0, PivotFilterType.ValueGreaterThan, 300, 0);

            // Beräkna och uppdatera data
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Spara arbetsboken
            workbook.Save("PivotTableColumnFieldsDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotFieldCollection](../../pivotfieldcollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


