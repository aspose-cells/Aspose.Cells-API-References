---
title: "ListObject.StartColumn"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListObject-egenskap. Hämtar startkolumnen för intervallet"
type: docs
url: /sv/net/aspose.cells.tables/listobject/startcolumn/
---
## ListObject.StartColumn property

Hämtar startkolumnen i intervallet.

```csharp
public int StartColumn { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyStartColumnDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa exempeldata för tabellen
            worksheet.Cells["E5"].PutValue("ID");
            worksheet.Cells["F5"].PutValue("Name");
            worksheet.Cells["G5"].PutValue("Age");
            
            worksheet.Cells["E6"].PutValue(1);
            worksheet.Cells["F6"].PutValue("John");
            worksheet.Cells["G6"].PutValue(30);
            
            worksheet.Cells["E7"].PutValue(2);
            worksheet.Cells["F7"].PutValue("Alice");
            worksheet.Cells["G7"].PutValue(25);

            // Skapa ett listobjekt (tabell)
            int startRow = 5;
            int startCol = 4; // Column E (0-based index 4)
            int endRow = 7;
            int endCol = 6; // Column G (0-based index 6)
            
            ListObject table = worksheet.ListObjects[worksheet.ListObjects.Add(startRow, startCol, endRow, endCol, true)];
            
            // Demonstrera StartColumn-egenskapen
            Console.WriteLine("Table starts at column index: " + table.StartColumn);
            Console.WriteLine("Table starts at column letter: " + CellsHelper.ColumnIndexToName(table.StartColumn));
            
            // Spara arbetsboken
            workbook.Save("ListObjectStartColumnDemo.xlsx");
        }
    }
}
```

### Se även

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


