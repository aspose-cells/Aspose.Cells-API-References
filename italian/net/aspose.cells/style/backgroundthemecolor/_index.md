---
title: "Style.BackgroundThemeColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Style. Ottiene e imposta il colore di tema di sfondo"
type: docs
url: /it/net/aspose.cells/style/backgroundthemecolor/
---
## Style.BackgroundThemeColor property

Ottiene e imposta il colore del tema di sfondo.

```csharp
public ThemeColor BackgroundThemeColor { get; set; }
```

### Osservazioni

Se il colore di sfondo non è un colore di tema, verrà restituito NULL.

### Esempi

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StylePropertyBackgroundThemeColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Crea uno stile e imposta il colore di tema di sfondo
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            
            ThemeColor themeColor = new ThemeColor(ThemeColorType.Accent2, 0.5);
            style.BackgroundThemeColor = themeColor;

            // Applica lo stile a una cella
            cells["A1"].SetStyle(style);

            // Verifica il colore di tema di sfondo
            ThemeColor retrievedColor = cells["A1"].GetStyle().BackgroundThemeColor;
            Console.WriteLine("Background Theme Color Type: " + retrievedColor.ColorType);
            Console.WriteLine("Background Theme Color Tint: " + retrievedColor.Tint);
        }
    }
}
```

### Vedi anche

* class [ThemeColor](../../themecolor/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


