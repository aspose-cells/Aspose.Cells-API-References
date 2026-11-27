---
title: "ListColumn.Formula"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListColumn egenskap. Hämtar och anger formeln för listkolumnen"
type: docs
url: /sv/net/aspose.cells.tables/listcolumn/formula/
---
## ListColumn.Formula property

Hämtar och anger formeln för listkolumnen.

```csharp
public string Formula { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListColumnPropertyFormulaDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Skapa exempeldata och tabell
            sheet.Cells["A1"].PutValue("Numbers");
            sheet.Cells["A2"].PutValue(5);
            sheet.Cells["A3"].PutValue(10);
            sheet.Cells["A4"].PutValue(15);
            
            sheet.Cells["B1"].PutValue("Doubled");
            sheet.Cells["B2"].PutValue("=A2*2");
            
            int tableIndex = sheet.ListObjects.Add(0, 0, 3, 1, true);
            ListObject table = sheet.ListObjects[tableIndex];
            table.ShowTotals = true;
            
            // Lägg till formel i listkolumnen
            ListColumn column = table.ListColumns[0];
            column.Formula = "=A2*3"; // This will apply to all cells in the column
            
            // Spara arbetsboken
            workbook.Save("ListColumnFormulaDemo.xlsx");
        }
    }
}
```

### Se även

* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


