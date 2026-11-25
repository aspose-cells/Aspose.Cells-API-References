---
title: "Font.ThemeColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Font. Ottiene e imposta il colore del tema"
type: docs
url: /it/net/aspose.cells/font/themecolor/
---
## Font.ThemeColor property

Ottiene e imposta il colore del tema.

```csharp
public ThemeColor ThemeColor { get; set; }
```

### Osservazioni

Se il colore del carattere non è un colore del tema, verrà restituito NULL.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyThemeColorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accedi alla cella A1 e imposta il testo
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Theme Color Demo");

            // Ottieni lo stile e il carattere
            Style style = cell.GetStyle();
            Font font = style.Font;

            // Crea e imposta il colore del tema
            font.ThemeColor = new ThemeColor(ThemeColorType.Accent1, 0.5);

            // Applica lo stile alla cella
            cell.SetStyle(style);

            // Salva la cartella di lavoro
            workbook.Save("ThemeColorDemo.xlsx");

            // Verifica il colore del tema
            Font savedFont = worksheet.Cells["A1"].GetStyle().Font;
            Console.WriteLine("ThemeColor Type: " + savedFont.ThemeColor.ColorType);
            Console.WriteLine("ThemeColor Tint: " + savedFont.ThemeColor.Tint);
        }
    }
}
```

### Vedi anche

* class [ThemeColor](../../themecolor/)
* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


