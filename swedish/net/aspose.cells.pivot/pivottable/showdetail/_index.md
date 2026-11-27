---
title: "PivotTable.ShowDetail"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-metod. Visa detaljerna för ett objekt i dataområdet i en ny tabell"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/showdetail/
---
## PivotTable.ShowDetail method

Visa detaljerna för ett objekt i dataområdet i en ny tabell.

```csharp
public void ShowDetail(int rowOffset, int columnOffset, bool newSheet, int destRow, int destColumn)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowOffset | Int32 | Avstånd till den första dataraden i dataområdet. |
| columnOffset | Int32 | Avstånd till den första datakolumnen i dataområdet. |
| newSheet | Boolean | Visa detaljerna i ett nytt kalkylblad. |
| destRow | Int32 | Målraden. |
| destColumn | Int32 | Målkolumnen. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodShowDetailWithInt32Int32BooleanInt32Int32Demo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för pivottabell
            worksheet.Cells["A1"].PutValue("Sport");
            worksheet.Cells["A2"].PutValue("Tennis");
            worksheet.Cells["A3"].PutValue("Basketball");
            worksheet.Cells["A4"].PutValue("Tennis");
            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["B2"].PutValue(80);
            worksheet.Cells["B3"].PutValue(90);
            worksheet.Cells["B4"].PutValue(85);

            // Skapa pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Sport");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Score");

            // Visa detaljer för en specifik cell
            pivotTable.ShowDetail(1, 0, true, 0, 0);

            // Spara arbetsboken
            workbook.Save("PivotTableShowDetailExample.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


