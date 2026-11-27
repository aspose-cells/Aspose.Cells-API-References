---
title: "PivotField.FilterTop10"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotField metod. Filtrerar efter värden i datapivotfältet"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfield/filtertop10/
---
## PivotField.FilterTop10 method

Filtrerar efter värden för data-pivotfält.

```csharp
public PivotFilter FilterTop10(int valueFieldIndex, PivotFilterType type, bool isTop, int itemCount)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| valueFieldIndex | Int32 | Index för datafältet i dataområdet. |
| typ | PivotFilterType | Typen av filtreringsdata. Kan endast vara Count, Sum och Percent. |
| isTop | Boolean | Anger om filtret är från toppen eller botten |
| itemCount | Int32 | Antalet objekt |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodFilterTop10WithInt32PivotFilterTypeBooleanIntDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för pivottabell
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["A5"].Value = "Apple";
            worksheet.Cells["A6"].Value = "Orange";
            worksheet.Cells["A7"].Value = "Banana";
            worksheet.Cells["A8"].Value = "Apple";
            
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 20;
            worksheet.Cells["B4"].Value = 30;
            worksheet.Cells["B5"].Value = 40;
            worksheet.Cells["B6"].Value = 50;
            worksheet.Cells["B7"].Value = 60;
            worksheet.Cells["B8"].Value = 70;

            // Skapa pivottabell
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B8", "C3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // Lägg till radfält
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // Lägg till datafält
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Tillämpa top 10-filter
            pivotTable.BaseFields[0].FilterTop10(0, PivotFilterType.Count, false, 2);
            
            // Spara arbetsboken
            workbook.Save("PivotTableFilterTop10.xlsx");
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


