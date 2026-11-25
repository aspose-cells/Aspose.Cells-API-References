---
title: "Style.ForegroundThemeColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Style. Ottiene e imposta il colore tematico di primo piano"
type: docs
url: /it/net/aspose.cells/style/foregroundthemecolor/
---
## Style.ForegroundThemeColor property

Ottiene e imposta il colore del tema in primo piano.

```csharp
public ThemeColor ForegroundThemeColor { get; set; }
```

### Osservazioni

Se il colore di primo piano non è un colore tematico, verrà restituito NULL.

### Esempi

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

### Vedi anche

* class [ThemeColor](../../themecolor/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


