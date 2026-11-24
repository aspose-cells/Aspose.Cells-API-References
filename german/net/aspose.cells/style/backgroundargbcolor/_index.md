---
title: "Style.BackgroundArgbColor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Style-Eigenschaft. Gibt die Hintergrundfarbe zurück und legt sie fest, wobei ein 32‑Bit‑ARGB‑Wert verwendet wird"
type: docs
url: /de/net/aspose.cells/style/backgroundargbcolor/
---
## Style.BackgroundArgbColor property

Liest und setzt die Hintergrundfarbe mit einem 32‑Bit‑ARGB‑Wert.

```csharp
public int BackgroundArgbColor { get; set; }
```

### Beispiele

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

### Siehe auch

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


