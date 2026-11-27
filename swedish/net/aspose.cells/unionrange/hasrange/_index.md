---
title: "UnionRange.HasRange"
second_title: "Aspose.Cells för .NET API‑referens"
description: "UnionRange‑egenskap. Indikerar om detta har ett område"
type: docs
url: /sv/net/aspose.cells/unionrange/hasrange/
---
## UnionRange.HasRange property

Indikerar om detta har ett område.

```csharp
public bool HasRange { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class UnionRangePropertyHasRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa ett unionområde med rätt API
            UnionRange unionRange = workbook.Worksheets.CreateUnionRange("A1:A5,B1:B5", 0);
            
            // Kontrollera om unionområdet har giltiga områden
            Console.WriteLine("UnionRange has ranges: " + unionRange.HasRange);
            
            // Ange värde och stil endast om området är giltigt
            if (unionRange.HasRange)
            {
                unionRange.Value = "Test Value";
                
                Style style = workbook.CreateStyle();
                style.Pattern = BackgroundType.Solid;
                style.ForegroundColor = System.Drawing.Color.LightBlue;
                unionRange.ApplyStyle(style, new StyleFlag { All = true });
            }
            
            workbook.Save("UnionRangeHasRangeDemo.xlsx");
        }
    }
}
```

### Se även

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


