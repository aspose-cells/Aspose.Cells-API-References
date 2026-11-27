---
title: "Cell.R1C1Formula"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell-egenskap. Hämtar eller anger en R1C1-formel för Cell"
type: docs
url: /sv/net/aspose.cells/cell/r1c1formula/
---
## Cell.R1C1Formula property

Hämtar eller anger en R1C1-formel för [`Cell`](../).

```csharp
public string R1C1Formula { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyR1C1FormulaDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ange A1-värde
            worksheet.Cells["A1"].PutValue(10);
            
            // Ange B1-värde
            worksheet.Cells["B1"].PutValue(20);
            
            // Ange C1-formel i A1-notation
            worksheet.Cells["C1"].Formula = "=A1+B1";
            
            // Hämta och visa R1C1-formel
            string r1c1Formula = worksheet.Cells["C1"].R1C1Formula;
            Console.WriteLine("R1C1 Formula: " + r1c1Formula);
            
            // Ange D1-formel i R1C1-notation
            worksheet.Cells["D1"].R1C1Formula = "=RC[-3]+RC[-2]";
            
            // Hämta och visa A1-formel
            string a1Formula = worksheet.Cells["D1"].Formula;
            Console.WriteLine("A1 Formula: " + a1Formula);
            
            // Spara arbetsboken
            workbook.Save("R1C1FormulaDemo.xlsx");
        }
    }
}
```

### Se även

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


