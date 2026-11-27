---
title: "FindOptions.GetRange"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FindOptions-metod. Hämtar och sätter det sökta intervallet"
type: docs
url: /sv/net/aspose.cells/findoptions/getrange/
---
## FindOptions.GetRange method

Hämtar och anger det sökta intervallet.

```csharp
public CellArea GetRange()
```

### Returvärde

Returnerar det sökta intervallet.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FindOptionsMethodGetRangeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll i lite exempeldata
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Cherry");
            worksheet.Cells["B1"].PutValue("Orange");
            worksheet.Cells["B2"].PutValue("Grape");
            worksheet.Cells["B3"].PutValue("Lemon");

            // Skapa en FindOptions-instans
            FindOptions findOptions = new FindOptions();
            findOptions.LookInType = LookInType.Values;
            findOptions.LookAtType = LookAtType.Contains;

            // Ställ in sökintervallet till A1:B3
            CellArea searchArea = new CellArea();
            searchArea.StartRow = 0;
            searchArea.StartColumn = 0;
            searchArea.EndRow = 2;
            searchArea.EndColumn = 1;
            findOptions.SetRange(searchArea);

            try
            {
                // Hämta intervallet som sattes
                CellArea resultRange = findOptions.GetRange();

                // Visa intervallinformationen
                Console.WriteLine($"Search range: StartRow={resultRange.StartRow}, StartColumn={resultRange.StartColumn}, " +
                    $"EndRow={resultRange.EndRow}, EndColumn={resultRange.EndColumn}");

                // Utför en sökoperation för att demonstrera att intervallet används
                Cell foundCell = worksheet.Cells.Find("an", null, findOptions);
                if (foundCell != null)
                {
                    Console.WriteLine($"Found value '{foundCell.StringValue}' at {foundCell.Name}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetRange method: {ex.Message}");
            }

            // Spara arbetsboken
            workbook.Save("MethodGetRangeDemo.xlsx");
        }
    }
}
```

### Se även

* struct [CellArea](../../cellarea/)
* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


