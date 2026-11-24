---
title: "Style.ForegroundThemeColor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Style-Eigenschaft. Gibt die Vordergrund-Theme-Farbe zurück und legt sie fest"
type: docs
url: /de/net/aspose.cells/style/foregroundthemecolor/
---
## Style.ForegroundThemeColor property

Liest und setzt die Vordergrund‑Themenfarbe.

```csharp
public ThemeColor ForegroundThemeColor { get; set; }
```

### Hinweise

Wenn die Vordergrundfarbe keine Theme-Farbe ist, wird NULL zurückgegeben.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyForegroundThemeColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            cells["A1"].PutValue("Foreground Theme Color Demo");
            Style style = cells["A1"].GetStyle();

            style.ForegroundThemeColor = new ThemeColor(ThemeColorType.Accent1, -0.25);
            style.Pattern = BackgroundType.Solid;

            cells["A1"].SetStyle(style);
            workbook.Save("ForegroundThemeColorDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ThemeColor](../../themecolor/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


