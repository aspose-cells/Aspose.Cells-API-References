---
title: "PivotAreaFilter.Selected"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotAreaFilter-egenskap. Anger om detta fält har en markering. Fungerar endast när pivottabellen är i konturvy"
type: docs
url: /sv/net/aspose.cells.pivot/pivotareafilter/selected/
---
## PivotAreaFilter.Selected property

Indikerar om detta fält har markering. Fungerar endast när pivottabellen är i översiktsvy.

```csharp
public bool Selected { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotAreaFilterPropertySelectedDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabell
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;

            // Skapa en pivottabell
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Hämta pivotområdefilter
            PivotArea pivotArea = new PivotArea(pivotTable);
            PivotAreaFilter filter = pivotArea.Filters[0];

            // Visa aktuellt valt värde
            Console.WriteLine("Current Selected value: " + filter.Selected);

            // Ändra valt värde (påverkar endast konturvy)
            filter.Selected = true;
            Console.WriteLine("New Selected value: " + filter.Selected);

            // Spara arbetsboken
            workbook.Save("PivotAreaFilterSelectedDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotAreaFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


