---
title: "GlobalizationSettings.GetStandardFunctionName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GlobalizationSettings‑metod. Hämtar standardfunktionsnamnet enligt angivet lokalt beroende funktionsnamn."
type: docs
url: /sv/net/aspose.cells/globalizationsettings/getstandardfunctionname/
---
## GlobalizationSettings.GetStandardFunctionName method

Hämtar standardfunktionsnamnet enligt givet lokalanpassat funktionsnamn.

```csharp
public virtual string GetStandardFunctionName(string localName)
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

    public class GlobalizationSettingsMethodGetStandardFunctionNameWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Förbered exempeldata
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["A2"].PutValue(15);
            
            // Skapa anpassade globaliseringsinställningar och tilldela dem till arbetsboken
            var customSettings = new CustomGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = customSettings;

            try
            {
                // Demonstrera GetStandardFunctionName med det tyska SUM-funktionsnamnet
                string localName = "SUMME";
                string standardName = customSettings.GetStandardFunctionName(localName);
                
                Console.WriteLine($"Local function name: {localName}");
                Console.WriteLine($"Standard function name: {standardName}");

                // Applicera lokalt funktionsnamn i formeln
                worksheet.Cells["A3"].Formula = "=SUMME(A1:A2)";
                workbook.CalculateFormula();
                
                Console.WriteLine($"Formula result: {worksheet.Cells["A3"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetStandardFunctionName method: {ex.Message}");
            }

            workbook.Save("MethodGetStandardFunctionNameDemo.xlsx");
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override string GetStandardFunctionName(string localName)
            {
                // Konvertera tysk funktionsnamn till standardengelska
                if (localName.Equals("SUMME", StringComparison.OrdinalIgnoreCase))
                {
                    return "SUM";
                }
                return base.GetStandardFunctionName(localName);
            }
        }
    }
}
```

### Se även

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


