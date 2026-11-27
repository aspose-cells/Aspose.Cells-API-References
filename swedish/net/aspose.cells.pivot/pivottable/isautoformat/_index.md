---
title: "PivotTable.IsAutoFormat"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable egenskap. Anger om PivotTable-rapporten är automatiskt formaterad. Kryssruta autoformat tabell som finns i pivottable-alternativ för Excel 2003"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/isautoformat/
---
## PivotTable.IsAutoFormat property

Anger om pivottabellsrapporten formateras automatiskt. Kryssrutan "autoformat table" som finns i pivottabellalternativet för Excel 2003.

```csharp
public bool IsAutoFormat { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyIsAutoFormatDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabell
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(150);

            // Lägg till en pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Konfigurera pivottabell
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");

            // Ställ in IsAutoFormat egenskap
            pivotTable.IsAutoFormat = true; // Enable auto formatting
            pivotTable.CalculateData();

            // Spara arbetsboken
            workbook.Save("PivotTableIsAutoFormatDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


