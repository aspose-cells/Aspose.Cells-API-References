---
title: "SettableGlobalizationSettings.SetStandardHeaderFooterFontStyleName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettableGlobalizationSettings‑metoden. Ställer in den lokalanpassade funktionsnamnet enligt det givna standardfunktionsnamnet"
type: docs
url: /sv/net/aspose.cells/settableglobalizationsettings/setstandardheaderfooterfontstylename/
---
## SettableGlobalizationSettings.SetStandardHeaderFooterFontStyleName method

Ställer in det lokalberoende funktionsnamnet enligt det givna standardfunktionsnamnet.

```csharp
public void SetStandardHeaderFooterFontStyleName(string localfontStyleName, string standardName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| localfontStyleName | String | Lokalt typsnittsstilnamn för Header/Footer. |
| standardName | String | Standard (en-US‑locale) funktionsnamn. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetStandardHeaderFooterFontStyleNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa sidinställningsalternativ för kalkylbladet
            PageSetup pageSetup = worksheet.PageSetup;

            // Ställ in ett sidhuvud med lite text
            pageSetup.SetHeader(0, "&\"Arial\"&12This is a header");

            // Skapa en instans av globaliseringsinställningar
            SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();

            try
            {
                // Anropa metoden SetStandardHeaderFooterFontStyleName
                globalizationSettings.SetStandardHeaderFooterFontStyleName("Arial", "Times New Roman");

                // Applicera globaliseringsinställningarna på arbetsboken
                workbook.Settings.GlobalizationSettings = globalizationSettings;

                Console.WriteLine("SetStandardHeaderFooterFontStyleName method executed successfully with parameters (\"Arial\", \"Times New Roman\")");

                // Effekten kommer att vara synlig när dokumentet renderas eller skrivs ut
                // Typsnittsstilen "Arial" i sidhuvuden/sidfötter kommer att behandlas som "Times New Roman"
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetStandardHeaderFooterFontStyleName method: {ex.Message}");
            }

            // Spara resultatet
            workbook.Save("MethodSetStandardHeaderFooterFontStyleNameDemo.xlsx");
        }
    }
}
```

### Se även

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


