---
title: "PivotField.ClearFilter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotField-metod. Rensar filterinställning på detta pivottfält"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfield/clearfilter/
---
## PivotField.ClearFilter method

Rensar filterinställningen för detta pivotfält.

```csharp
public void ClearFilter()
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldMethodClearFilterDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabell
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["A2"].Value = "Fruit";
            worksheet.Cells["A3"].Value = "Vegetable";
            worksheet.Cells["A4"].Value = "Fruit";
            worksheet.Cells["A5"].Value = "Vegetable";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 150;
            worksheet.Cells["B5"].Value = 300;

            // Skapa pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Lägg till radfält
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            
            // Lägg till datafält
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Hämta pivotfältet
            PivotField pivotField = pivotTable.RowFields[0];

            try
            {
                // Applicera ett filter först för att demonstrera hur man rensar det
                pivotField.FilterByLabel(PivotFilterType.CaptionEqual, "Fruit", null);

                // Anropa ClearFilter-metoden
                pivotField.ClearFilter();

                Console.WriteLine("ClearFilter method executed successfully");
                Console.WriteLine("All filters have been removed from the pivot field");

                // Uppdatera pivottabellen för att visa ändringarna
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ClearFilter method: {ex.Message}");
            }

            // Spara resultatet
            workbook.Save("PivotFieldMethodClearFilterDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


