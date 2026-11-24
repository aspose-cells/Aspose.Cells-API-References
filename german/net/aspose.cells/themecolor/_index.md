---
title: "Klasse ThemeColor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.ThemeColor Klasse. Stellt eine Themenfarbe dar"
type: docs
url: /de/net/aspose.cells/themecolor/
---
## ThemeColor class

Stellt eine Themenfarbe dar.

```csharp
public class ThemeColor
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [ThemeColor](themecolor/)(ThemeColorType, double) |  |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [ColorType](../../aspose.cells/themecolor/colortype/) { get; set; } | Liest und setzt den Thementyp. |
| [Tint](../../aspose.cells/themecolor/tint/) { get; set; } | Liest und setzt den Tönungswert. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThemeColorDemo
    {
        public static void ThemeColorExample()
        {
            // Instanziieren eines Workbook-Objekts
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Wert zu Zelle A1 hinzufügen
            cells["A1"].PutValue("Hello World");

            // Stil von Zelle A1 abrufen
            Style style = cells["A1"].GetStyle();

            // Setze ThemeColorType.Text2 Farbtyp mit 40 % Aufhellung als Schriftfarbe.
            style.Font.ThemeColor = new ThemeColor(ThemeColorType.Text2, 0.4);
            style.Pattern = BackgroundType.Solid;

            // Setze ThemeColorType.Background2 Farbtyp mit 75 % Abdunkelung als Vordergrundfarbe.
            style.ForegroundThemeColor = new ThemeColor(ThemeColorType.Background2, -0.75);

            // Den Stil auf Zelle A1 anwenden
            cells["A1"].SetStyle(style);

            // Die Excel-Datei speichern
            workbook.Save("ThemeColorExample.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


