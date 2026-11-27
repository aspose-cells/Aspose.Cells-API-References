---
title: "GlobalizationSettings.GetStandardHeaderFooterFontStyleName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GlobalizationSettings-metoden. Hämtar standardengelskt typsnittsstilsnamn Regular Bold Italic för Header/Footer enligt angivet lokala typsnittsstilsnamn"
type: docs
url: /sv/net/aspose.cells/globalizationsettings/getstandardheaderfooterfontstylename/
---
## GlobalizationSettings.GetStandardHeaderFooterFontStyleName method

Hämtar standardengelskt teckensnittsstilsnamn (Regular, Bold, Italic) för Header/Footer enligt given lokalanpassat teckensnittsstilsnamn.

```csharp
public virtual string GetStandardHeaderFooterFontStyleName(string localfontStyleName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| localfontStyleName | String | Lokalt typsnittsstilnamn för Header/Footer. |

### Returvärde

Standardengelskt typsnittsstilnamn (Regular, Bold, Italic)

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsMethodGetStandardHeaderFooterFontStyleNameWithStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en anpassad instans av GlobalizationSettings
            var globalizationSettings = new CustomGlobalizationSettings();

            try
            {
                // Demonstrera metodanrop med parametertyp (String)
                string localStyle = "CustomBold";
                string standardStyle = globalizationSettings.GetStandardHeaderFooterFontStyleName(localStyle);
                Console.WriteLine($"Converted font style: {localStyle} -> {standardStyle}");

                // Applicera globaliseringsinställningar på arbetsboken
                workbook.Settings.GlobalizationSettings = globalizationSettings;

                // Ställ in header med anpassad typsnittsstil som kommer att konverteras
                // Använd SetHeader-metoden med sektionparameter (0 = vänster, 1 = centrum, 2 = höger)
                worksheet.PageSetup.SetHeader(1, "&\"Arial\"&\"CustomBold\"&12Header Text");

                // Spara arbetsboken för att visa effekten
                workbook.Save("MethodGetStandardHeaderFooterFontStyleNameDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetStandardHeaderFooterFontStyleName method: {ex.Message}");
            }
        }
    }

    // Implementering av anpassade globaliseringsinställningar
    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetStandardHeaderFooterFontStyleName(string localfontStyleName)
        {
            // Konvertera anpassade typsnittsstilsnamn till standardnamn
            return localfontStyleName switch
            {
                "CustomBold" => "Bold",
                "CustomItalic" => "Italic",
                _ => base.GetStandardHeaderFooterFontStyleName(localfontStyleName)
            };
        }
    }
}
```

### Se även

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


