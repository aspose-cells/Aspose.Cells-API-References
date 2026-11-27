---
title: "FindOptions.SearchOrderByRows"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FindOptions-egenskapen. Anger om sökordningen är efter rader eller kolumner"
type: docs
url: /sv/net/aspose.cells/findoptions/searchorderbyrows/
---
## FindOptions.SearchOrderByRows property

Anger om sökordningen är efter rader eller kolumner.

```csharp
public bool SearchOrderByRows { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertySearchOrderByRowsDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok och lägg till exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fyll celler med testdata (söker efter \"abc\" i kolumnordning)
            worksheet.Cells["A1"].PutValue("xyz");
            worksheet.Cells["B1"].PutValue("def");
            worksheet.Cells["A2"].PutValue("123");
            worksheet.Cells["B2"].PutValue("abc");
            worksheet.Cells["A3"].PutValue("abc");
            worksheet.Cells["B3"].PutValue("789");

            // Skapa sökalternativ och ange sökordning till kolumnordning
            FindOptions findOptions = new FindOptions();
            findOptions.SearchOrderByRows = false; // Search column by column

            // Sök \"abc\" - bör returnera A3 (rad 2, kolumn 0) vid kolumnordning
            Cell foundCell = worksheet.Cells.Find("abc", null, findOptions);

            // Skriv ut resultatet
            Console.WriteLine($"Found 'abc' at row: {foundCell.Row}, column: {foundCell.Column}");
        }
    }
}
```

### Se även

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


