---
title: "WorksheetCollection.GetNamedRangesAndTables"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorksheetCollection-metod. Hämtar alla fördefinierade namngivna områden i kalkylbladet"
type: docs
url: /sv/net/aspose.cells/worksheetcollection/getnamedrangesandtables/
---
## WorksheetCollection.GetNamedRangesAndTables method

Hämtar alla fördefinierade namngivna områden i kalkylbladet.

```csharp
public Range[] GetNamedRangesAndTables()
```

### Returvärde

En array av Range-objekt.

Returnerar null om det namngivna området inte finns.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodGetNamedRangesAndTablesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa några namngivna områden
            worksheet.Cells.CreateRange("A1:B2").Name = "TestRange1";
            worksheet.Cells.CreateRange("C3:D4").Name = "TestRange2";
            
            // Hämta alla namngivna områden och tabeller
            Aspose.Cells.Range[] ranges = workbook.Worksheets.GetNamedRangesAndTables();
            
            // Visa information om områdena
            Console.WriteLine("Found {0} named ranges:", ranges.Length);
            foreach (Aspose.Cells.Range range in ranges)
            {
                Console.WriteLine("Name: {0}, Address: {1}", range.Name, range.Address);
            }
        }
    }
}
```

### Se även

* class [Range](../../range/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


