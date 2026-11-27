---
title: "Style.ForegroundColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Style-egenskap. Hämtar eller anger stilens förgrundsfärg"
type: docs
url: /sv/net/aspose.cells/style/foregroundcolor/
---
## Style.ForegroundColor property

Hämtar eller anger en stils förgrundsfärg.

```csharp
public Color ForegroundColor { get; set; }
```

### Anmärkningar

Det betyder ingen färginställning om Color.Empty returneras.

### Exempel

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StylePropertyForegroundColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            Style style = workbook.CreateStyle();
            style.ForegroundColor = Color.Green;
            style.Pattern = BackgroundType.Solid;
            
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            
            Console.WriteLine("ForegroundColor set to: " + style.ForegroundColor);
            
            workbook.Save("ForegroundColorDemo.xlsx");
        }
    }
}
```

### Se även

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


