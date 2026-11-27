---
title: "Range.RefersTo"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Range-egenskap. Hämtar vad området refererar till"
type: docs
url: /sv/net/aspose.cells/range/refersto/
---
## Range.RefersTo property

Hämtar vad området refererar till.

```csharp
public string RefersTo { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyRefersToDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till lite data i cellerna
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            
            // Skapa ett namngivet område
            int index = workbook.Worksheets.Names.Add("MyRange");
            Name name = workbook.Worksheets.Names[index];
            
            // Ställ in RefersTo-egenskapen för det namngivna området
            name.RefersTo = "=Sheet1!$A$1:$A$3";
            
            // Hämta de områden som refereras av namnet
            Aspose.Cells.Range[] ranges = name.GetRanges();
            
            // Visa RefersTo-egenskapen för det första området
            Console.WriteLine("Named range refers to: " + ranges[0].RefersTo);
            
            // Skapa en formel som använder det namngivna området
            worksheet.Cells["B1"].Formula = "=SUM(MyRange)";
            
            // Beräkna formeln
            Console.WriteLine("Sum of named range: " + worksheet.Cells["B1"].Value);
        }
    }
}
```

### Se även

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


