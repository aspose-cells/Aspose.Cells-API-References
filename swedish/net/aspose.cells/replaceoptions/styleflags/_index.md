---
title: "ReplaceOptions.StyleFlags"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ReplaceOptions egenskap. Hämtar och anger flaggor för tillämpning av teckensnittsinställningar"
type: docs
url: /sv/net/aspose.cells/replaceoptions/styleflags/
---
## ReplaceOptions.StyleFlags property

Hämtar och anger flaggor för att tillämpa teckensnittsinställningar.

```csharp
public StyleFlag[] StyleFlags { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ReplaceOptionsPropertyStyleFlagsDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeltext i cellen
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("test text");

            // Skapa ersättningsalternativ
            ReplaceOptions options = new ReplaceOptions();
            options.MatchEntireCellContents = false;
            options.CaseSensitive = false;

            // Skapa teckensnittsinställning och stilflagg
            string replacementText = "new text";
            FontSetting setting = new FontSetting(0, replacementText.Length, workbook.Worksheets);
            StyleFlag styleFlag = new StyleFlag();
            
            // Konfigurera teckensnitt och stil
            setting.Font.Color = Color.Red;
            setting.Font.Underline = FontUnderlineType.Single;
            styleFlag.FontColor = true;
            styleFlag.FontUnderline = true;

            // Tillämpa inställningarna på alternativen
            options.FontSettings = new FontSetting[] { setting };
            options.StyleFlags = new StyleFlag[] { styleFlag };

            // Utför ersättning
            workbook.Replace("test", replacementText, options);

            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [StyleFlag](../../styleflag/)
* class [ReplaceOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


