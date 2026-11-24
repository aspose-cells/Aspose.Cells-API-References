---
title: "ReplaceOptions.FontSettings"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ReplaceOptions-Eigenschaft. Die reich formatierte Einstellung für den ersetzten Text"
type: docs
url: /de/net/aspose.cells/replaceoptions/fontsettings/
---
## ReplaceOptions.FontSettings property

Die reich formatierten Einstellungen für den ersetzten Text.

```csharp
public FontSetting[] FontSettings { get; set; }
```

### Beispiele

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
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieltext in Zelle A1 festlegen
            worksheet.Cells["A1"].Value = "Sample text for replacement";
            
            // Ersetzungsoptionen mit Schrifteinstellungen erstellen
            ReplaceOptions options = new ReplaceOptions();
            options.MatchEntireCellContents = false;
            
            // Schrifteinstellung für den Ersetzungstext erstellen
            FontSetting fontSetting = new FontSetting(0, 8, workbook.Worksheets);
            fontSetting.Font.IsBold = true;
            fontSetting.Font.Color = Color.Blue;
            
            // Schrifteinstellungen auf Ersetzungsoptionen anwenden
            options.FontSettings = new FontSetting[] { fontSetting };
            
            // Ersetzung ausführen
            workbook.Replace("text", "REPLACED", options);
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [FontSetting](../../fontsetting/)
* class [ReplaceOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


