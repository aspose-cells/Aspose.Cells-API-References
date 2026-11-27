---
title: "PivotFilterCollection.AddTop10Filter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotFilterCollection metod. Filtrerar efter värden i datapivotfältet"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfiltercollection/addtop10filter/
---
## PivotFilterCollection.AddTop10Filter method

Filtrerar efter värden för data-pivotfält.

```csharp
public PivotFilter AddTop10Filter(int baseFieldIndex, int valueFieldIndex, PivotFilterType type, 
    bool isTop, int itemCount)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| baseFieldIndex | Int32 | Indexet för fältet i källan. |
| valueFieldIndex | Int32 | Index för datafältet i dataområdet. |
| typ | PivotFilterType | Typen av filtreringsdata. Kan endast vara Count, Sum och Percent. |
| isTop | Boolean | Anger om filtret är från toppen eller botten |
| itemCount | Int32 | Antalet objekt |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFilterCollectionMethodAddTop10FilterWithInt32Int32PivotFilterTypeBooleDemo
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
            worksheet.Cells["A4"].Value = "Dairy";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 150;
            worksheet.Cells["B3"].Value = 80;
            worksheet.Cells["B4"].Value = 120;

            // Skapa pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Lägg till radfält
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            
            // Lägg till datafält
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            try
            {
                // Hämta samling av pivotfilter
                PivotFilterCollection filters = pivotTable.PivotFilters;
                
                // Lägg till Top10-filter - visa de 2 bästa artiklarna efter försäljning
                PivotFilter filter = filters.AddTop10Filter(
                    baseFieldIndex: 0,          // Category field
                    valueFieldIndex: 1,          // Sales field
                    type: PivotFilterType.Count, // Filter type
                    isTop: true,                 // Show top items
                    itemCount: 2                 // Number of items to show
                );

                Console.WriteLine($"Top10 filter added successfully. Filter type: {filter.FilterType}");
                Console.WriteLine($"Field index: {filter.FieldIndex}, Value field index: {filter.ValueFieldIndex}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error adding Top10 filter: {ex.Message}");
            }
            
            // Spara arbetsboken
            workbook.Save("PivotFilterCollectionMethodAddTop10FilterDemo.xlsx");
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


