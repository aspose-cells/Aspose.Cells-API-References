---
title: "ThemeColor.Tint"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ThemeColor-egenskap. Hämtar och anger nyansvärdet"
type: docs
url: /sv/net/aspose.cells/themecolor/tint/
---
## ThemeColor.Tint property

Hämtar och anger nyansvärdet.

```csharp
public double Tint { get; set; }
```

### Anmärkningar

Nyansvärdet lagras som ett double‑värde från -1,0 till 1,0, där -1,0 betyder 100 % mörkare och 1,0 betyder 100 % ljusare. Dessutom betyder 0,0 ingen förändring.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThemeColorPropertyTintDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en stil med temafärg och nyans
            Style style = workbook.CreateStyle();
            style.BackgroundThemeColor = new ThemeColor(ThemeColorType.Accent1, 0.5); // 0.5 tint
            
            // Tillämpa stilen på en cell
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);

            // Hämta nyansvärdet från cellens stil
            double tintValue = cell.GetStyle().BackgroundThemeColor.Tint;
            Console.WriteLine("Tint value: " + tintValue);

            // Ändra nyansvärdet
            ThemeColor themeColor = cell.GetStyle().BackgroundThemeColor;
            themeColor.Tint = 0.8; // Change tint to 0.8
            cell.SetStyle(style);

            // Verifiera det nya nyansvärdet
            Console.WriteLine("Modified tint value: " + cell.GetStyle().BackgroundThemeColor.Tint);
        }
    }
}
```

### Se även

* class [ThemeColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


