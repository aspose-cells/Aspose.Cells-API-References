---
title: "Workbook.SetThemeColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-metod. Ställer in temafärgen"
type: docs
url: /sv/net/aspose.cells/workbook/setthemecolor/
---
## Workbook.SetThemeColor method

Ställer in temafärgen

```csharp
public void SetThemeColor(ThemeColorType type, Color color)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| typ | ThemeColorType | Temafärgstypen. |
| färg | Färg | temafärgen |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Ställ in temafärgen för Text1 till Grön
            workbook.SetThemeColor(ThemeColorType.Text1, Color.Green);
            
            // Tillämpa temafärgen på standardstilen
            Style style = workbook.DefaultStyle;
            style.Font.ThemeColor = new ThemeColor(ThemeColorType.Text1, 0);
            workbook.DefaultStyle = style;
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
            
            Console.WriteLine("Workbook with theme color saved successfully.");
        }
    }
}
```

### Se även

* enum [ThemeColorType](../../themecolortype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


