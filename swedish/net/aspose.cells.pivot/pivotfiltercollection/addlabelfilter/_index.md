---
title: "PivotFilterCollection.AddLabelFilter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotFilterCollection‑metod. Filtrerar efter rubriker för rad‑ eller kolumn‑pivotfält"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfiltercollection/addlabelfilter/
---
## PivotFilterCollection.AddLabelFilter method

Filtrerar efter rubriker för rad- eller kolumn-pivotfält.

```csharp
public PivotFilter AddLabelFilter(int baseFieldIndex, PivotFilterType type, string label1, 
    string label2)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| baseFieldIndex | Int32 | Indexet för fältet i källan. |
| typ | PivotFilterType | Typen av filtreringsdata. |
| label1 | String | Etiketten för filtervillkoret |
| label2 | String | Den övre gränsetiketten för mellanfiltervillkoret |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFilterCollectionMethodAddLabelFilterWithInt32PivotFilterTypeStringStriDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabell
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["A4"].Value = "Cherry";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

            // Skapa pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Lägg till radfält
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            
            // Lägg till datafält
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            try
            {
                PivotFilterCollection filters = pivotTable.PivotFilters;
                
                // Lägg till etikettfilter för att visa produkter som börjar med "A"
                PivotFilter filter = filters.AddLabelFilter(
                    baseFieldIndex: 0,
                    type: PivotFilterType.CaptionBeginsWith,
                    label1: "A",
                    label2: null
                );

                Console.WriteLine($"Label filter added successfully. Filter type: {filter.FilterType}");
                Console.WriteLine($"Field index: {filter.FieldIndex}, Value1: {filter.Value1}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error adding label filter: {ex.Message}");
            }
            
            workbook.Save("PivotFilterCollectionMethodAddLabelFilterDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotFilter](../../pivotfilter/)
* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotFilterCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


