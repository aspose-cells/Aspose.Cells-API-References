---
title: "Style.ForegroundColor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Style-Eigenschaft. Gibt die Vordergrundfarbe eines Stils zurück oder legt sie fest"
type: docs
url: /de/net/aspose.cells/style/foregroundcolor/
---
## Style.ForegroundColor property

Liest oder setzt die Vordergrundfarbe eines Stils.

```csharp
public Color ForegroundColor { get; set; }
```

### Hinweise

Das bedeutet, dass keine Farbe eingestellt ist, wenn Color.Empty zurückgegeben wird.

### Beispiele

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

### Siehe auch

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


