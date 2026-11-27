---
title: "SettableGlobalizationSettings.GetStandardHeaderFooterFontStyleName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettableGlobalizationSettings metod. Hämtar standardengelsk typsnittsstilnamn Regular Bold Italic för Header/Footer enligt det angivna lokala typsnittsstilnamnet"
type: docs
url: /sv/net/aspose.cells/settableglobalizationsettings/getstandardheaderfooterfontstylename/
---
## SettableGlobalizationSettings.GetStandardHeaderFooterFontStyleName method

Hämtar standardengelskt teckensnittsstilsnamn (Regular, Bold, Italic) för Header/Footer enligt given lokalanpassat teckensnittsstilsnamn.

```csharp
public override string GetStandardHeaderFooterFontStyleName(string localfontStyleName)
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

    public class SettableGlobalizationSettingsMethodGetStandardHeaderFooterFontStyleNameWithStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa anpassade globaliseringsinställningar
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // Ställ in en standardmappning för header/footer-typsnittsstilnamn
            settings.SetStandardHeaderFooterFontStyleName("MyLocalFontStyle", "Arial");

            // Applicera inställningarna på arbetsboken
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // Anropa metoden GetStandardHeaderFooterFontStyleName med ett lokalt typsnittsstilnamn
                string standardFontStyle = settings.GetStandardHeaderFooterFontStyleName("MyLocalFontStyle");
                
                // Visa resultatet
                Console.WriteLine($"Standard font style name for 'MyLocalFontStyle': {standardFontStyle}");

                // Skapa ett header med det lokala typsnittsstilnamnet
                worksheet.PageSetup.SetHeader(1, "&\"MyLocalFontStyle\"&12Test Header");

                // Visa effekten i kalkylbladet
                Console.WriteLine("Header set with local font style name 'MyLocalFontStyle'");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetStandardHeaderFooterFontStyleName method: {ex.Message}");
            }
            
            // Spara resultatet
            workbook.Save("MethodGetStandardHeaderFooterFontStyleNameDemo.xlsx");
        }
    }
}
```

### Se även

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


