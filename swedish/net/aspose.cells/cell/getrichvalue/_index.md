---
title: "Cell.GetRichValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell-metod. Hämtar det rika värdet för cellen"
type: docs
url: /sv/net/aspose.cells/cell/getrichvalue/
---
## Cell.GetRichValue method

Hämtar cellens rika värde.

```csharp
public CellRichValue GetRichValue()
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetRichValueDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook wb = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet ws = wb.Worksheets[0];
            
            // Ange ett rikt textvärde i cell A1
            ws.Cells["A1"].PutValue("This is rich text");
            
            // Hämta det rika värdet från cell A1
            CellRichValue richValue = ws.Cells["A1"].GetRichValue();
            
            // Visa det rika textvärdet
            Console.WriteLine("Rich Text Value: " + ws.Cells["A1"].StringValue);
            
            // Spara arbetsboken
            wb.Save("RichValueDemo.xlsx");
        }
    }
}
```

### Se även

* class [CellRichValue](../../cellrichvalue/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


