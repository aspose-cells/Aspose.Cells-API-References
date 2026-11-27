---
title: "PivotFilterCollection.AddDateFilter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotFilterCollection metod. Filtrerar efter datuminställning för rad- eller kolumnpivotfält"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfiltercollection/adddatefilter/
---
## PivotFilterCollection.AddDateFilter method

Filtrerar efter datuminställning för rad- eller kolumn-pivotfält.

```csharp
public PivotFilter AddDateFilter(int baseFieldIndex, PivotFilterType type, DateTime dateTime1, 
    DateTime dateTime2)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| baseFieldIndex | Int32 | Indexet för fältet i källan. |
| typ | PivotFilterType | Typen av filtreringsdata. |
| dateTime1 | DateTime | Datumetiketten för filtervillkoret |
| dateTime2 | DateTime | Den övre datumetiketten för mellanfiltervillkoret |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFilterCollectionMethodAddDateFilterWithInt32PivotFilterTypeDateTimeDaDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata med datum
            worksheet.Cells["A1"].Value = "Date";
            worksheet.Cells["A2"].Value = new DateTime(2023, 1, 15);
            worksheet.Cells["A3"].Value = new DateTime(2023, 2, 20);
            worksheet.Cells["A4"].Value = new DateTime(2023, 3, 10);
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;

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
                
                // Lägg till datumfilter för att visa datum mellan 1 januari och 31 mars 2023
                PivotFilter filter = filters.AddDateFilter(
                    baseFieldIndex: 0,
                    type: PivotFilterType.DateBetween,
                    dateTime1: new DateTime(2023, 1, 1),
                    dateTime2: new DateTime(2023, 3, 31)
                );

                Console.WriteLine($"Date filter added successfully. Filter type: {filter.FilterType}");
                Console.WriteLine($"Field index: {filter.FieldIndex}, UseWholeDay: {filter.UseWholeDay}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error adding date filter: {ex.Message}");
            }
            
            workbook.Save("PivotFilterCollectionMethodAddDateFilterDemo.xlsx");
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


