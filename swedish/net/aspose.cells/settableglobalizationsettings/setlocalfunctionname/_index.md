---
title: "SettableGlobalizationSettings.SetLocalFunctionName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettableGlobalizationSettings-metoden. Anger det lokalanpassade funktionsnamnet som motsvarar det givna standardfunktionsnamnet"
type: docs
url: /sv/net/aspose.cells/settableglobalizationsettings/setlocalfunctionname/
---
## SettableGlobalizationSettings.SetLocalFunctionName method

Ställer in det lokalberoende funktionsnamnet som motsvarar det givna standardfunktionsnamnet.

```csharp
public void SetLocalFunctionName(string standardName, string localName, bool bidirectional)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| standardName | String | Standard (en-US‑locale) funktionsnamn. |
| localName | String | Lokalberoende funktionsnamn |
| bidirectional | Boolean | Om den lokala funktionsnamnet ska mappas till standardfunktionsnamnet automatiskt. Om true kommer det lokala namnet att mappas till standardnamnet automatiskt så att användaren inte behöver anropa [`SetStandardFunctionName`](../setstandardfunctionname/) igen för samma par av standard- och lokala namn. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetLocalFunctionNameWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa globaliseringsinställningar
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            try
            {
                // Anropa SetLocalFunctionName för att mappa standardfunktionsnamnet till det lokala namnet
                settings.SetLocalFunctionName("SUM", "SOMMA", true); // Italian localization for SUM function
                settings.SetLocalFunctionName("AVERAGE", "MEDIA", true); // Italian localization for AVERAGE function

                // Applicera inställningarna på arbetsboken
                workbook.Settings.GlobalizationSettings = settings;

                // Skapa formler som använder både standard- och lokalanpassade namn
                worksheet.Cells["A1"].Formula = "=SUM(B1:B5)";
                worksheet.Cells["A2"].Formula = "=SOMMA(B1:B5)";
                worksheet.Cells["A3"].Formula = "=AVERAGE(B1:B5)";
                worksheet.Cells["A4"].Formula = "=MEDIA(B1:B5)";

                // Beräkna formler
                workbook.CalculateFormula();

                Console.WriteLine("SetLocalFunctionName executed successfully with parameters (String, String, Boolean)");
                Console.WriteLine("Standard and localized function names work equivalently in formulas.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetLocalFunctionName method: {ex.Message}");
            }

            // Spara resultatet
            workbook.Save("MethodSetLocalFunctionNameWithStringStringBooleanDemo.xlsx");
        }
    }
}
```

### Se även

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


