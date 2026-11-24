---
title: "ThemeColor.Tint"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ThemeColor Eigenschaft. Liest und setzt den Farbtonwert"
type: docs
url: /de/net/aspose.cells/themecolor/tint/
---
## ThemeColor.Tint property

Liest und setzt den Tönungswert.

```csharp
public double Tint { get; set; }
```

### Hinweise

Der Farbtonwert wird als Double von -1,0 bis 1,0 gespeichert, wobei -1,0 100% Abdunkeln und 1,0 100% Aufhellen bedeutet. Außerdem bedeutet 0,0 keine Änderung.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThemeColorPropertyTintDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle einen Stil mit Themenfarbe und Farbton
            Style style = workbook.CreateStyle();
            style.BackgroundThemeColor = new ThemeColor(ThemeColorType.Accent1, 0.5); // 0.5 tint
            
            // Wende den Stil auf eine Zelle an
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);

            // Hole den Farbtonwert aus dem Zellenstil
            double tintValue = cell.GetStyle().BackgroundThemeColor.Tint;
            Console.WriteLine("Tint value: " + tintValue);

            // Den Farbtonwert ändern
            ThemeColor themeColor = cell.GetStyle().BackgroundThemeColor;
            themeColor.Tint = 0.8; // Change tint to 0.8
            cell.SetStyle(style);

            // Den neuen Farbtonwert überprüfen
            Console.WriteLine("Modified tint value: " + cell.GetStyle().BackgroundThemeColor.Tint);
        }
    }
}
```

### Siehe auch

* class [ThemeColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


