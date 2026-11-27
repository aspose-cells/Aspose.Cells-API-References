---
title: "CellArea.EndRow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CellArea-fält. Hämtar eller anger den sista raden i detta område"
type: docs
url: /sv/net/aspose.cells/cellarea/endrow/
---
## CellArea.EndRow field

Hämtar eller anger slutraden för detta område.

```csharp
public int EndRow;
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class CellAreaFieldEndRowDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för pivottabell
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(150);
            
            // Lägg till pivottabell
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Lägg till radfält och datafält
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Demonstrera användning av EndRow
            Console.WriteLine("Pivot table ends at row: " + pivotTable.TableRange2.EndRow);
            
            // Spara arbetsboken
            workbook.Save("PivotTable_EndRow_Demo.xlsx");
        }
    }
}
```

### Se även

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


