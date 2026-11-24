---
title: "WorkbookSettings.GetThemeFont"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings method. Gibt den Namen der Standardschriftart des Themas zurück"
type: docs
url: /de/net/aspose.cells/workbooksettings/getthemefont/
---
## WorkbookSettings.GetThemeFont method

Ruft den Standard‑Themen‑Schriftartnamen ab.

```csharp
public string GetThemeFont(FontSchemeType type)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Typ | FontSchemeType | Der Schematyp der Schriftart. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsMethodGetThemeFontWithFontSchemeTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Rufe die Standardschriftart des Themas für den Minor-Schema-Typ ab
            string minorFont = workbook.Settings.GetThemeFont(FontSchemeType.Minor);
            Console.WriteLine("Minor theme font: " + minorFont);
            
            // Rufe die Standardschriftart des Themas für den Major-Schema-Typ ab
            string majorFont = workbook.Settings.GetThemeFont(FontSchemeType.Major);
            Console.WriteLine("Major theme font: " + majorFont);
            
            // Speichere die Arbeitsmappe
            workbook.Save("ThemeFontExample.xlsx");
        }
    }
}
```

### Siehe auch

* enum [FontSchemeType](../../fontschemetype/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


