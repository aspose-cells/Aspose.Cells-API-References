---
title: "Cell.DateTimeValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell-egenskap. Hämtar DateTime-värdet som finns i cellen"
type: docs
url: /sv/net/aspose.cells/cell/datetimevalue/
---
## Cell.DateTimeValue property

Hämtar DateTime‑värdet som finns i cellen.

```csharp
public DateTime DateTimeValue { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyDateTimeValueDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ange ett DateTime-värde i cell A1
            DateTime testDate = new DateTime(2023, 12, 25);
            cells["A1"].PutValue(testDate);

            // Formatera cellen för att visa datum
            Style style = cells["A1"].GetStyle();
            style.Custom = "yyyy-MM-dd";
            cells["A1"].SetStyle(style);

            // Hämta och verifiera DateTimeValue
            DateTime retrievedDate = cells["A1"].DateTimeValue;
            Console.WriteLine("Original DateTime: " + testDate.ToString("yyyy-MM-dd"));
            Console.WriteLine("Retrieved DateTime: " + retrievedDate.ToString("yyyy-MM-dd"));

            // Ange ett annat DateTime-värde i cell B1
            DateTime anotherDate = new DateTime(2024, 1, 1);
            cells["B1"].PutValue(anotherDate);

            // Visa DateTimeValue från B1
            Console.WriteLine("B1 DateTime: " + cells["B1"].DateTimeValue.ToString("yyyy-MM-dd"));
        }
    }
}
```

### Se även

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


