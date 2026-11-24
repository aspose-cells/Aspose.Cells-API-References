---
title: "Workbook.GetThemeColor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook‑Methode. Ruft die Themenfarbe ab"
type: docs
url: /de/net/aspose.cells/workbook/getthemecolor/
---
## Workbook.GetThemeColor method

Ermittelt die Designfarbe.

```csharp
public Color GetThemeColor(ThemeColorType type)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Typ | ThemeColorType | Der Typ der Themenfarbe. |

### Rückgabewert

Die Themenfarbe.

### Beispiele

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodGetThemeColorWithThemeColorTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Themenfarbe für Accent6 abrufen
            Color color = workbook.GetThemeColor(ThemeColorType.Accent6);
            Console.WriteLine("Theme Color (Accent6): " + color.ToString());
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* enum [ThemeColorType](../../themecolortype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


