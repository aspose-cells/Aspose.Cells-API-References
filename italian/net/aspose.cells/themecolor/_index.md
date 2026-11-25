---
title: "Classe ThemeColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.ThemeColor. Rappresenta un colore del tema"
type: docs
url: /it/net/aspose.cells/themecolor/
---
## ThemeColor class

Rappresenta un colore del tema.

```csharp
public class ThemeColor
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [ThemeColor](themecolor/)(ThemeColorType, double) |  |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [ColorType](../../aspose.cells/themecolor/colortype/) { get; set; } | Ottiene e imposta il tipo di tema. |
| [Tint](../../aspose.cells/themecolor/tint/) { get; set; } | Ottiene e imposta il valore della tinta. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThemeColorDemo
    {
        public static void ThemeColorExample()
        {
            // Istanziare un oggetto Workbook
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Aggiunta di un valore alla cella A1
            cells["A1"].PutValue("Hello World");

            // Recupero dello stile della cella A1
            Style style = cells["A1"].GetStyle();

            // Imposta il tipo di colore ThemeColorType.Text2 con un chiarimento del 40% come colore del carattere.
            style.Font.ThemeColor = new ThemeColor(ThemeColorType.Text2, 0.4);
            style.Pattern = BackgroundType.Solid;

            // Imposta il tipo di colore ThemeColorType.Background2 con un'oscuramento del 75% come colore di primo piano.
            style.ForegroundThemeColor = new ThemeColor(ThemeColorType.Background2, -0.75);

            // Applicazione dello stile alla cella A1
            cells["A1"].SetStyle(style);

            // Salvataggio del file Excel
            workbook.Save("ThemeColorExample.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


