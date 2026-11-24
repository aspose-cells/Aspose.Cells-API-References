---
title: "ReplaceOptions.StyleFlags"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ReplaceOptions-Eigenschaft. Gibt und setzt Flags für die Anwendung von Schriftarteinstellungen"
type: docs
url: /de/net/aspose.cells/replaceoptions/styleflags/
---
## ReplaceOptions.StyleFlags property

Liest und setzt Flags für die Anwendung von Schriftarteinstellungen.

```csharp
public StyleFlag[] StyleFlags { get; set; }
```

### Beispiele

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
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieltext zur Zelle hinzufügen
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("test text");

            // Ersetzungsoptionen erstellen
            ReplaceOptions options = new ReplaceOptions();
            options.MatchEntireCellContents = false;
            options.CaseSensitive = false;

            // Schrifteinstellung und Stil-Flag erstellen
            string replacementText = "new text";
            FontSetting setting = new FontSetting(0, replacementText.Length, workbook.Worksheets);
            StyleFlag styleFlag = new StyleFlag();
            
            // Schrift und Stil konfigurieren
            setting.Font.Color = Color.Red;
            setting.Font.Underline = FontUnderlineType.Single;
            styleFlag.FontColor = true;
            styleFlag.FontUnderline = true;

            // Einstellungen auf Optionen anwenden
            options.FontSettings = new FontSetting[] { setting };
            options.StyleFlags = new StyleFlag[] { styleFlag };

            // Ersetzung durchführen
            workbook.Replace("test", replacementText, options);

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [StyleFlag](../../styleflag/)
* class [ReplaceOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


