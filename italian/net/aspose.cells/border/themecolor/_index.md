---
title: "Border.ThemeColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Border. Ottiene e imposta il colore del tema del bordo"
type: docs
url: /it/net/aspose.cells/border/themecolor/
---
## Border.ThemeColor property

Ottiene e imposta il colore tematico del bordo.

```csharp
public ThemeColor ThemeColor { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BorderPropertyThemeColorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accedi a una cella e ottieni il suo stile
            Style style = worksheet.Cells["A1"].GetStyle();

            // Imposta il colore del tema del bordo
            style.Borders[BorderType.BottomBorder].ThemeColor = new ThemeColor(ThemeColorType.Accent1, 0.5);
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;

            // Applica lo stile alla cella
            worksheet.Cells["A1"].SetStyle(style);

            // Salva la cartella di lavoro
            workbook.Save("BorderThemeColorDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ThemeColor](../../themecolor/)
* class [Border](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


