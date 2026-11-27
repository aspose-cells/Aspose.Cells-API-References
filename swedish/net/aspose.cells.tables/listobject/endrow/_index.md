---
title: "ListObject.EndRow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListObject‑egenskap. Hämtar den sista raden i intervallet"
type: docs
url: /sv/net/aspose.cells.tables/listobject/endrow/
---
## ListObject.EndRow property

Hämtar den sista raden i intervallet.

```csharp
public int EndRow { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyEndRowDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Skapa exempeldata
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["B1"].PutValue("Age");
            sheet.Cells["A2"].PutValue("John");
            sheet.Cells["B2"].PutValue(30);
            sheet.Cells["A3"].PutValue("Mary");
            sheet.Cells["B3"].PutValue(25);
            
            // Skapa listobjekt/tabell
            int idx = sheet.ListObjects.Add(0, 0, 3, 1, true);
            ListObject table = sheet.ListObjects[idx];
            
            // Visa initial EndRow
            Console.WriteLine("Initial EndRow: " + table.EndRow);
            
            // Lägg till ny rad i tabellen
            table.PutCellValue(4, 0, "Tom");
            table.PutCellValue(4, 1, 28);
            
            // Visa uppdaterad EndRow
            Console.WriteLine("Updated EndRow: " + table.EndRow);
            
            // Spara arbetsboken
            wb.Save("ListObjectEndRowDemo.xlsx");
        }
    }
}
```

### Se även

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


