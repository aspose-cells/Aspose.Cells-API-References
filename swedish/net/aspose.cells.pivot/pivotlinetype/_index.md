---
title: "Enum PivotLineType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Pivot.PivotLineType enum. Anger typen av PivotLine"
type: docs
url: /sv/net/aspose.cells.pivot/pivotlinetype/
---
## PivotLineType enumeration

Anger typen för PivotLine.

```csharp
public enum PivotLineType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Regular | `0` | Vanlig PivotLine med pivotelement. |
| Subtotal | `1` | Delsumma‑rad. |
| GrandTotal | `2` | Summa‑rad. |
| Blank | `3` | Tom rad efter varje grupp. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotClassPivotLineTypeDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för pivottabell
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(300);

            // Skapa pivottabell
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Lägg till radfält och datafält
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Sortera radfältet efter värden i fallande ordning
            pivotTable.RowFields[0].SortBy(SortOrder.Descending, 0, PivotLineType.Regular, "B2");
            
            // Beräkna pivottabellsdata
            pivotTable.CalculateData();
            
            // Spara arbetsboken
            workbook.Save("PivotLineTypeDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


