---
title: "Cell.GetTable"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell-metod. Hämtar tabellen som innehåller den här cellen"
type: docs
url: /sv/net/aspose.cells/cell/gettable/
---
## Cell.GetTable method

Hämtar tabellen som innehåller den här cellen.

```csharp
public ListObject GetTable()
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class CellMethodGetTableDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Skapa en tabell med rubriker och data
            cells["A1"].PutValue("Product");
            cells["B1"].PutValue("Price");
            cells["A2"].PutValue("Apple");
            cells["B2"].PutValue(2.5);
            cells["A3"].PutValue("Orange");
            cells["B3"].PutValue(1.8);

            // Skapa ett ListObject (tabell) från dataområdet
            int tableIndex = worksheet.ListObjects.Add("A1", "B3", true);
            ListObject table = worksheet.ListObjects[tableIndex];

            // Demonstrera GetTable-metoden
            Cell cellInTable = cells["B2"];
            ListObject resultTable = cellInTable.GetTable();
            
            Console.WriteLine("Table found: " + (resultTable != null));
            Console.WriteLine("Table range: " + resultTable.StartRow + "," + resultTable.StartColumn + 
                            " to " + resultTable.EndRow + "," + resultTable.EndColumn);
        }
    }
}
```

### Se även

* class [ListObject](../../../aspose.cells.tables/listobject/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


