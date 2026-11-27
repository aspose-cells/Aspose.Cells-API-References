---
title: "ReplaceOptions.FontSettings"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ReplaceOptions egenskap. De rikformatterade inställningarna för den ersatta texten"
type: docs
url: /sv/net/aspose.cells/replaceoptions/fontsettings/
---
## ReplaceOptions.FontSettings property

De rikligt formaterade inställningarna för den ersatta texten.

```csharp
public FontSetting[] FontSettings { get; set; }
```

### Exempel

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReplaceOptionsPropertyFontSettingsDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ställ in exempeltext i cell A1
            worksheet.Cells["A1"].Value = "Sample text for replacement";
            
            // Skapa ersättningsalternativ med teckensnittsinställningar
            ReplaceOptions options = new ReplaceOptions();
            options.MatchEntireCellContents = false;
            
            // Skapa teckensnittsinställning för ersättningstexten
            FontSetting fontSetting = new FontSetting(0, 8, workbook.Worksheets);
            fontSetting.Font.IsBold = true;
            fontSetting.Font.Color = Color.Blue;
            
            // Tillämpa teckensnittsinställningar på ersättningsalternativen
            options.FontSettings = new FontSetting[] { fontSetting };
            
            // Utför ersättningen
            workbook.Replace("text", "REPLACED", options);
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [FontSetting](../../fontsetting/)
* class [ReplaceOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


