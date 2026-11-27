---
title: "ListObject.EndColumn"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListObject-egenskap. Hämtar slutkolumnen för området"
type: docs
url: /sv/net/aspose.cells.tables/listobject/endcolumn/
---
## ListObject.EndColumn property

Hämtar den sista kolumnen i intervallet.

```csharp
public int EndColumn { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyEndColumnDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["C1"].PutValue("Age");
            for (int i = 2; i <= 5; i++)
            {
                worksheet.Cells[$"A{i}"].PutValue(i-1);
                worksheet.Cells[$"B{i}"].PutValue($"Person {i-1}");
                worksheet.Cells[$"C{i}"].PutValue(20 + i);
            }

            // Skapa ett listobjekt/tabell
            int listObjectIndex = worksheet.ListObjects.Add(0, 0, 4, 2, true);
            ListObject table = worksheet.ListObjects[listObjectIndex];
            table.ShowTotals = true;
            
            // Visa den ursprungliga slutkolumnen
            Console.WriteLine($"Original EndColumn: {table.EndColumn}");
            
            // Ändra storlek på tabellen så att den inkluderar en extra kolumn
            table.Resize(table.StartRow, table.StartColumn, table.EndRow, table.EndColumn + 1, table.ShowHeaderRow);
            
            // Visa den nya slutkolumnen
            Console.WriteLine($"New EndColumn: {table.EndColumn}");
            
            // Spara arbetsboken
            workbook.Save("ListObjectEndColumnDemo.xlsx");
        }
    }
}
```

### Se även

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


