---
title: "StyleFlag.FontColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "StyleFlag property. Inställningen för teckensnittsfärg kommer att tillämpas"
type: docs
url: /sv/net/aspose.cells/styleflag/fontcolor/
---
## StyleFlag.FontColor property

Inställning för teckensnittsfärg kommer att tillämpas.

```csharp
public bool FontColor { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyFontColorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa en anpassad stil
            Style style = workbook.CreateStyle();
            style.Font.Color = System.Drawing.Color.Red;
            style.BackgroundColor = System.Drawing.Color.LightGray;
            
            // Skapa en stilflagga och aktivera teckensnittsfärg och cellskuggning
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.FontColor = true;
            styleFlag.CellShading = true;
            
            // Applicera stilen på cell A1 med de angivna flaggorna
            worksheet.Cells["A1"].PutValue("Red Text on Gray Background");
            worksheet.Cells["A1"].SetStyle(style, styleFlag);
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


