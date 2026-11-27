---
title: "PivotTable.NullString"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-egenskap. Hämtar strängen som visas i celler som innehåller nullvärden när egenskapen DisplayNullString är sann. Standardvärdet är en tom sträng"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/nullstring/
---
## PivotTable.NullString property

Hämtar strängen som visas i celler som innehåller null‑värden när egenskapen DisplayNullString är true. Standardvärdet är en tom sträng.

```csharp
public string NullString { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyNullStringDemo
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
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 1000;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 2000;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 3000;
            cells["A5"].Value = null; // Null value
            cells["B5"].Value = 4000;

            // Skapa pivottabell
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Lägg till fält i pivottabell
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Ställ in NullString-egenskapen och visningsinställningarna
            pivotTable.NullString = "(null)";
            pivotTable.DisplayNullString = true;

            // Uppdatera pivot‑tabellens data
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Spara arbetsboken
            workbook.Save("PivotTableNullStringDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


