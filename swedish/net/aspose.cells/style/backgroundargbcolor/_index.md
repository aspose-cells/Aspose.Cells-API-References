---
title: "Style.BackgroundArgbColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Style property. Hämtar och anger bakgrundsfärgen med ett 32‑bitars ARGB‑värde"
type: docs
url: /sv/net/aspose.cells/style/backgroundargbcolor/
---
## Style.BackgroundArgbColor property

Hämtar och anger bakgrundsfärgen med ett 32‑bitars ARGB‑värde.

```csharp
public int BackgroundArgbColor { get; set; }
```

### Exempel

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyBackgroundArgbColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            
            Style style = cell.GetStyle();
            style.BackgroundArgbColor = Color.Yellow.ToArgb();
            style.Pattern = BackgroundType.Solid;
            
            cell.SetStyle(style);
            cell.PutValue("Sample Text with Yellow Background");
            
            workbook.Save("BackgroundArgbColorDemo.xlsx");
        }
    }
}
```

### Se även

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


