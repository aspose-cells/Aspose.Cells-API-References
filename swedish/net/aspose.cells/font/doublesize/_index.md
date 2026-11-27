---
title: "Font.DoubleSize"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Font-egenskap. Hämtar och anger dubbel storlek på teckensnittet"
type: docs
url: /sv/net/aspose.cells/font/doublesize/
---
## Font.DoubleSize property

Hämtar och anger dubbel storlek på teckensnittet.

```csharp
public double DoubleSize { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyDoubleSizeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            
            Style style = cell.GetStyle();
            style.Font.DoubleSize = 10.5;
            cell.SetStyle(style);
            
            Console.WriteLine("Font DoubleSize set to: " + cell.GetStyle().Font.DoubleSize);
        }
    }
}
```

### Se även

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


