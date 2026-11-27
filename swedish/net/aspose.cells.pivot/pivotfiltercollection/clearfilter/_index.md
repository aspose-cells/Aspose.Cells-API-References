---
title: "PivotFilterCollection.ClearFilter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotFilterCollection‑metod. Rensa PivotFilter från det specifika PivotField"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfiltercollection/clearfilter/
---
## PivotFilterCollection.ClearFilter method

Rensa PivotFilter från den specifika PivotField

```csharp
public void ClearFilter(int fieldIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldIndex | Int32 | PivotField‑indexet |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFilterCollectionMethodClearFilterWithInt32Demo
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
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 5;
            worksheet.Cells["B4"].Value = 8;

            // Skapa pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Lägg till radfält
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            
            // Lägg till datafält
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Lägg till filter till pivottabell
            PivotFilterCollection filters = pivotTable.PivotFilters;
            filters.AddLabelFilter(0, PivotFilterType.Count, "Apple", null);

            try
            {
                // Anropa ClearFilter‑metoden med fält‑indexparameter
                filters.ClearFilter(0);
                
                Console.WriteLine("Pivot filter cleared successfully for field index 0");
                
                // Verifiera att filtret rensades
                Console.WriteLine($"Number of filters after clearing: {filters.Count}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ClearFilter method: {ex.Message}");
            }
            
            // Spara arbetsboken
            workbook.Save("PivotFilterCollectionMethodClearFilterWithInt32Demo.xlsx");
        }
    }
}
```

### Se även

* class [PivotFilterCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


