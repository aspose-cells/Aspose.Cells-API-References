---
title: "FindOptions.IsRangeSet"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FindOptions-egenskap. Anger om det sökta intervallet är satt"
type: docs
url: /sv/net/aspose.cells/findoptions/israngeset/
---
## FindOptions.IsRangeSet property

Anger om det sökta intervallet är angivet.

```csharp
public bool IsRangeSet { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FindOptionsPropertyIsRangeSetDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll i lite data
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Cherry");
            worksheet.Cells["B1"].PutValue("Date");
            worksheet.Cells["B2"].PutValue("Elderberry");
            worksheet.Cells["B3"].PutValue("Fig");

            // Skapa en FindOptions-instans
            FindOptions findOptions = new FindOptions();

            // Kontrollera initialt IsRangeSet‑värde (bör vara falskt)
            Console.WriteLine("Initial IsRangeSet value: " + findOptions.IsRangeSet);

            // Ställ in ett sökintervall
            CellArea searchRange = new CellArea();
            searchRange.StartRow = 0;
            searchRange.StartColumn = 0;
            searchRange.EndRow = 2;
            searchRange.EndColumn = 0; // Column A only
            findOptions.SetRange(searchRange);

            // Kontrollera IsRangeSet efter att intervallet satts (bör vara sant)
            Console.WriteLine("After SetRange, IsRangeSet value: " + findOptions.IsRangeSet);

            // Utför en sökoperation inom det angivna intervallet
            Cell foundCell = worksheet.Cells.Find("Banana", null, findOptions);
            Console.WriteLine("Found 'Banana' at: " + foundCell?.Name);

            // Försök att hitta något utanför intervallet (bör inte hittas)
            foundCell = worksheet.Cells.Find("Fig", null, findOptions);
            Console.WriteLine("Found 'Fig' at: " + foundCell?.Name); // Should be null

            // Spara arbetsboken
            workbook.Save("PropertyIsRangeSetDemo.xlsx");
        }
    }
}
```

### Se även

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


