---
title: "Cell.IsNumericValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell-egenskap. Anger om värdet i den här cellen är numeriskt, int, double och datetime"
type: docs
url: /sv/net/aspose.cells/cell/isnumericvalue/
---
## Cell.IsNumericValue property

Anger om värdet i den här cellen är numeriskt (int, double och datetime).

```csharp
public bool IsNumericValue { get; }
```

### Anmärkningar

Gäller också för formelceller för att kontrollera det beräknade resultatet

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsNumericValueDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till olika typer av data i celler
            Cell cell1 = worksheet.Cells["A1"];
            cell1.PutValue(123.45); // Numeric value

            Cell cell2 = worksheet.Cells["A2"];
            cell2.PutValue("Hello World"); // String value

            // Kontrollera om celler innehåller numeriska värden
            Console.WriteLine("Cell A1 IsNumericValue: " + cell1.IsNumericValue);
            Console.WriteLine("Cell A2 IsNumericValue: " + cell2.IsNumericValue);

            // Demonstrera användning med villkorslogik
            if (cell1.IsNumericValue)
            {
                Console.WriteLine("Cell A1 contains a numeric value: " + cell1.DoubleValue);
            }

            if (!cell2.IsNumericValue)
            {
                Console.WriteLine("Cell A2 does not contain a numeric value");
            }
        }
    }
}
```

### Se även

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


