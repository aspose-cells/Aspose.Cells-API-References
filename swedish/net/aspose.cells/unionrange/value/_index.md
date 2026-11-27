---
title: "UnionRange.Value"
second_title: "Aspose.Cells för .NET API‑referens"
description: "UnionRange‑egenskap. Hämtar och sätter värdena för området"
type: docs
url: /sv/net/aspose.cells/unionrange/value/
---
## UnionRange.Value property

Hämtar och anger värdena för området.

```csharp
public object Value { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class UnionRangePropertyValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa ett unionområde med rätt API
            UnionRange unionRange = workbook.Worksheets.CreateUnionRange("A1:B2,D1:E2", 0);
            
            // Ange värde för hela unionområdet
            unionRange.Value = "Test Value";
            
            // Skapa och tillämpa stil
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = System.Drawing.Color.LightBlue;
            unionRange.ApplyStyle(style, new StyleFlag { All = true });
            
            // Spara arbetsboken
            workbook.Save("UnionRangeValueDemo.xlsx");
        }
    }
}
```

### Se även

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


