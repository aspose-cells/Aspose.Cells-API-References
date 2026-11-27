---
title: "SettableGlobalizationSettings.GetStandardFunctionName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettableGlobalizationSettings-metod. Hämtar standardfunktionsnamnet enligt givet lokalt beroende funktionsnamn"
type: docs
url: /sv/net/aspose.cells/settableglobalizationsettings/getstandardfunctionname/
---
## SettableGlobalizationSettings.GetStandardFunctionName method

Hämtar standardfunktionsnamnet enligt givet lokalanpassat funktionsnamn.

```csharp
public override string GetStandardFunctionName(string localName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| localName | String | Locale‑beroende funktionsnamn. Språkinställningen angavs av arbetsboken för vilken dessa inställningar används. |

### Returvärde

Standard (en-US‑locale) funktionsnamn.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodGetStandardFunctionNameWithStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa anpassade globaliseringsinställningar
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // Ställ in en lokal funktionsnamnsmappning
            settings.SetStandardFunctionName("LocalSum", "SUM", true);

            // Applicera inställningarna på arbetsboken
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // Anropa GetStandardFunctionName med ett lokalt funktionsnamn
                string standardName = settings.GetStandardFunctionName("LocalSum");
                
                // Visa resultatet
                Console.WriteLine($"Standard function name for 'LocalSum' is: {standardName}");

                // Använd standardfunktionen i en cellformel
                worksheet.Cells["A1"].Formula = $"={standardName}(1,2,3)";
                worksheet.Cells["A2"].Value = 1;
                worksheet.Cells["A3"].Value = 2;
                worksheet.Cells["A4"].Value = 3;

                // Beräkna formeln
                workbook.CalculateFormula();

                // Visa resultatet
                Console.WriteLine($"Formula result in A1: {worksheet.Cells["A1"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetStandardFunctionName method: {ex.Message}");
            }
            
            // Spara arbetsboken
            workbook.Save("SettableGlobalizationSettingsMethodGetStandardFunctionNameWithStringDemo.xlsx");
        }
    }
}
```

### Se även

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


