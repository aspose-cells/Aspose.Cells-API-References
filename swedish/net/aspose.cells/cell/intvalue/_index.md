---
title: "Cell.IntValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell egenskap. Hämtar heltalsvärdet som finns i cellen"
type: docs
url: /sv/net/aspose.cells/cell/intvalue/
---
## Cell.IntValue property

Hämtar heltalsvärdet som finns i cellen.

```csharp
public int IntValue { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIntValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Ange ett numeriskt värde och hämta IntValue
            Cell cell1 = cells[0, 0];
            cell1.PutValue(42);
            Console.WriteLine("IntValue of numeric cell: " + cell1.IntValue);

            // Ange en formel som utvärderas till ett tal och hämta IntValue
            Cell cell2 = cells[0, 1];
            cell2.Formula = "=10+5";
            workbook.CalculateFormula();
            Console.WriteLine("IntValue of formula cell: " + cell2.IntValue);

            // Ange ett booleskt värde och hämta IntValue
            Cell cell3 = cells[0, 2];
            cell3.PutValue(true);
            Console.WriteLine("IntValue of boolean cell: " + cell3.IntValue);

            // Ange ett textvärde och hämta IntValue (blir 0 om det inte kan konverteras)
            Cell cell4 = cells[0, 3];
            cell4.PutValue("Hello");
            Console.WriteLine("IntValue of text cell: " + cell4.IntValue);
        }
    }
}
```

### Se även

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


