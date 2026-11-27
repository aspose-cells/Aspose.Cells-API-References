---
title: "PivotField.FilterByLabel"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotField-metod. Filtrerar efter rubriker för rad- eller kolumnpivotfält"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfield/filterbylabel/
---
## PivotField.FilterByLabel method

Filtrerar efter rubriker för rad- eller kolumn-pivotfält.

```csharp
public PivotFilter FilterByLabel(PivotFilterType type, string label1, string label2)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| typ | PivotFilterType | Typen av filtreringsdata. |
| label1 | String | Etiketten för filtervillkoret |
| label2 | String | Den övre gränsetiketten för mellanfiltervillkoret |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodFilterByLabelWithPivotFilterTypeStringStringDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("");
            sheet.Cells["A5"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);
            sheet.Cells["B5"].PutValue(40);

            // Skapa pivottabell med korrekta parametrar
            int pivotIndex = sheet.PivotTables.Add("A1:B5", "D1", "PivotTable");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            
            pivot.AddFieldToArea(PivotFieldType.Row, "Category");
            pivot.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Hämta pivotfältet
            PivotField field = pivot.RowFields[0];
            
            // Tillämpa filter
            field.FilterByLabel(PivotFilterType.CaptionNotEqual, "(blank)", "");
            pivot.RefreshData();
            pivot.CalculateData();
            
            // Spara arbetsboken
            workbook.Save("PivotFilterByLabelDemo.xlsx");
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


