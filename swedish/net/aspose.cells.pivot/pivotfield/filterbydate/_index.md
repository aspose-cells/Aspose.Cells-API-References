---
title: "PivotField.FilterByDate"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotField metod. Filtrerar efter datumvärden för rad- eller kolumnpivotfältet"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfield/filterbydate/
---
## PivotField.FilterByDate method

Filtrerar efter datumvärden för rad- eller kolumnpivotfält.

```csharp
public PivotFilter FilterByDate(PivotFilterType type, DateTime dateTime1, DateTime dateTime2)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| typ | PivotFilterType | Typen av filtreringsdata. |
| dateTime1 | DateTime | Datumetiketten för filtervillkoret |
| dateTime2 | DateTime | Den övre datumetiketten för mellanfiltervillkoret |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodFilterByDateWithPivotFilterTypeDateTimeDateTimDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata med datum
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(new DateTime(2020, 9, 15));
            worksheet.Cells["A3"].PutValue(new DateTime(2020, 10, 20));
            worksheet.Cells["A4"].PutValue(new DateTime(2021, 9, 16));
            worksheet.Cells["A5"].PutValue(new DateTime(2021, 11, 5));

            // Skapa pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:A5", "D3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Lägg till datumfält i kolumnområdet
            int fieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Column, 0);
            PivotField pivotField = pivotTable.ColumnFields[fieldIndex];
            
            // Applicera datumfilter (septemberdatum mellan 2020‑2021)
            pivotField.FilterByDate(PivotFilterType.September, new DateTime(2020, 1, 1), new DateTime(2021, 12, 31));
            
            // Uppdatera och beräkna pivottabell
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Spara resultat
            workbook.Save("FilterByDateDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotFilter](../../pivotfilter/)
* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


