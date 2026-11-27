---
title: "Workbook.GetThemeColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-metod. Hämtar temafärg"
type: docs
url: /sv/net/aspose.cells/workbook/getthemecolor/
---
## Workbook.GetThemeColor method

Hämtar temafärg.

```csharp
public Color GetThemeColor(ThemeColorType type)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| typ | ThemeColorType | Temafärgstypen. |

### Returvärde

Temafärgen.

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Hämta temafärg för Accent6
            Color color = workbook.GetThemeColor(ThemeColorType.Accent6);
            Console.WriteLine("Theme Color (Accent6): " + color.ToString());
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* enum [ThemeColorType](../../themecolortype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


