---
title: "GlobalizationSettings.GetStandardBuiltInName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GlobalizationSettings-metoden. Hämtar standardtexten för inbyggt namn enligt given lokalanpassad text"
type: docs
url: /sv/net/aspose.cells/globalizationsettings/getstandardbuiltinname/
---
## GlobalizationSettings.GetStandardBuiltInName method

Hämtar standardtexten för inbyggt namn enligt given lokalanpassad text.

```csharp
public virtual string GetStandardBuiltInName(string localName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| localName | String | Localespecifik text för inbyggt namn. Språkinställningen angavs av arbetsboken som dessa inställningar används för. |

### Returvärde

Standardtext (en-US-locale).

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsMethodGetStandardBuiltInNameWithStringDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med anpassade globaliseringsinställningar
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Initiera anpassade globaliseringsinställningar och tilldela dem till arbetsboken
            var globalizationSettings = new CustomGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = globalizationSettings;

            // Testparameter för GetStandardBuiltInName
            string localFunctionName = "MyLocalSum";
            
            try
            {
                // Anropa GetStandardBuiltInName med lokalt funktionsnamn
                string standardName = globalizationSettings.GetStandardBuiltInName(localFunctionName);
                Console.WriteLine($"Local name: '{localFunctionName}' => Standard name: '{standardName}'");

                // Demonstrera effekten genom att använda det lokala namnet i en formel
                worksheet.Cells["A1"].Value = 5;
                worksheet.Cells["A2"].Value = 7;
                worksheet.Cells["A3"].Formula = $"{localFunctionName}(A1:A2)";

                // Beräkna formel för att visa korrekt tolkning
                workbook.CalculateFormula();
                Console.WriteLine($"Formula result: {worksheet.Cells["A3"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetStandardBuiltInName: {ex.Message}");
            }

            // Spara den modifierade arbetsboken
            workbook.Save("GlobalizationGetStandardBuiltInNameDemo.xlsx");
        }
    }

    // Anpassade globaliseringsinställningar som åsidosätter GetStandardBuiltInName
    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetStandardBuiltInName(string localName)
        {
            // Mappa anpassat lokalt funktionsnamn till standard SUM
            if (localName.Equals("MyLocalSum", StringComparison.OrdinalIgnoreCase))
            {
                return "SUM";
            }
            return base.GetStandardBuiltInName(localName);
        }
    }
}
```

### Se även

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


