---
title: "Cells.StandardHeight"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-egenskap. Hämtar eller anger standardradens höjd i detta kalkylblad i enheten punkter"
type: docs
url: /sv/net/aspose.cells/cells/standardheight/
---
## Cells.StandardHeight property

Hämtar eller anger standardradshöjden i detta kalkylblad, i enheten punkter.

```csharp
public double StandardHeight { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyStandardHeightDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hämta och visa standardhöjden
            double standardHeight = worksheet.Cells.StandardHeight;
            Console.WriteLine("Standard Height: " + standardHeight);
            
            // Ange en ny standardhöjd
            worksheet.Cells.StandardHeight = 20;
            Console.WriteLine("New Standard Height: " + worksheet.Cells.StandardHeight);
            
            // Spara arbetsboken
            workbook.Save("StandardHeightDemo.xlsx");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


