---
title: "Workbook.SetThemeColor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook-Methode. Legt die Themenfarbe fest"
type: docs
url: /de/net/aspose.cells/workbook/setthemecolor/
---
## Workbook.SetThemeColor method

Setzt die Designfarbe

```csharp
public void SetThemeColor(ThemeColorType type, Color color)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Typ | ThemeColorType | Der Typ der Themenfarbe. |
| Farbe | Farbe | die Themenfarbe |

### Beispiele

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodSetThemeColorWithThemeColorTypeColorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Setze die Themenfarbe für Text1 auf Grün
            workbook.SetThemeColor(ThemeColorType.Text1, Color.Green);
            
            // Wende die Themenfarbe auf den Standardstil an
            Style style = workbook.DefaultStyle;
            style.Font.ThemeColor = new ThemeColor(ThemeColorType.Text1, 0);
            workbook.DefaultStyle = style;
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
            
            Console.WriteLine("Workbook with theme color saved successfully.");
        }
    }
}
```

### Siehe auch

* enum [ThemeColorType](../../themecolortype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


