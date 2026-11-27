---
title: "Worksheet.ListObjects"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet‑egenskap. Hämtar alla ListObjects i detta kalkylblad"
type: docs
url: /sv/net/aspose.cells/worksheet/listobjects/
---
## Worksheet.ListObjects property

Hämtar alla ListObjects i detta kalkylblad.

```csharp
public ListObjectCollection ListObjects { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyListObjectsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);
            
            // Skapa ett ListObject (tabell)
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[index];
            table.DisplayName = "ProductTable";
            table.ShowTotals = true;
            
            // Ändra storlek på tabellen för att inkludera fler rader
            table.Resize(table.StartRow, table.StartColumn, 5, table.EndColumn, true);
            
            // Lägg till mer data i den utökade tabellen
            worksheet.Cells["A4"].PutValue("Item3");
            worksheet.Cells["B4"].PutValue(300);
            worksheet.Cells["A5"].PutValue("Item4");
            worksheet.Cells["B5"].PutValue(400);
            
            // Kom åt tabellen via ListObjects‑egenskapen
            ListObject retrievedTable = worksheet.ListObjects["ProductTable"];
            retrievedTable.ShowHeaderRow = true;
            
            // Spara arbetsboken
            workbook.Save("ListObjectsDemo.xlsx");
        }
    }
}
```

### Se även

* class [ListObjectCollection](../../../aspose.cells.tables/listobjectcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


