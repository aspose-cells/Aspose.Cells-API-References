---
title: "WorkbookSettings.GetThemeFont"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings-metod. Hämtar standardtema typsnittets namn"
type: docs
url: /sv/net/aspose.cells/workbooksettings/getthemefont/
---
## WorkbookSettings.GetThemeFont method

Hämtar standardtemats typsnittsnamn.

```csharp
public string GetThemeFont(FontSchemeType type)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| typ | FontSchemeType | Typsnittets schematyp. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsMethodGetThemeFontWithFontSchemeTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Hämta standardtema‑typsnittet för mindre schematyp
            string minorFont = workbook.Settings.GetThemeFont(FontSchemeType.Minor);
            Console.WriteLine("Minor theme font: " + minorFont);
            
            // Hämta standardtema‑typsnittet för större schematyp
            string majorFont = workbook.Settings.GetThemeFont(FontSchemeType.Major);
            Console.WriteLine("Major theme font: " + majorFont);
            
            // Spara arbetsboken
            workbook.Save("ThemeFontExample.xlsx");
        }
    }
}
```

### Se även

* enum [FontSchemeType](../../fontschemetype/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


