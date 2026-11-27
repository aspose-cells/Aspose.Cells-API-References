---
title: "Klass CellRichValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.CellRichValue-klass. Representerar cellens rika värde."
type: docs
url: /sv/net/aspose.cells/cellrichvalue/
---
## CellRichValue class

Representerar cellens rikvärde.

```csharp
public abstract class CellRichValue
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| virtual [AltText](../../aspose.cells/cellrichvalue/alttext/) { get; set; } | Hämtar alternativ text som är associerad med bilden. |
| virtual [ErrorValue](../../aspose.cells/cellrichvalue/errorvalue/) { get; } | Hämtar felvärdestypen för cellen. |
| virtual [Image](../../aspose.cells/cellrichvalue/image/) { get; } | Hämtar bilddata för cellen. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassCellRichValueDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ställ in ett rikt värde i cell A1
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Rich Value");
            
            // Hämta det rika värdet från cell A1
            CellRichValue richValue = cell.GetRichValue();
            
            // Visa egenskaperna för det rika värdet
            Console.WriteLine("Rich Value: " + richValue.ToString());
            
            // Spara arbetsboken
            workbook.Save("RichValueDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


