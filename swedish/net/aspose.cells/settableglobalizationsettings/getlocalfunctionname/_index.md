---
title: "SettableGlobalizationSettings.GetLocalFunctionName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettableGlobalizationSettings-metod. Hämtar det lokalanpassade funktionsnamnet enligt angivet standardfunktionsnamn"
type: docs
url: /sv/net/aspose.cells/settableglobalizationsettings/getlocalfunctionname/
---
## SettableGlobalizationSettings.GetLocalFunctionName method

Hämtar det lokalanpassade funktionsnamnet enligt given standardfunktionsnamn.

```csharp
public override string GetLocalFunctionName(string standardName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| standardName | String | Standard (en-US‑locale) funktionsnamn. |

### Returvärde

Locale‑beroende funktionsnamn. Språkinställningen angavs av arbetsboken för vilken dessa inställningar används.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodGetLocalFunctionNameWithStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa anpassade globaliseringsinställningar
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // Ange ett anpassat lokalt funktionsnamn för "SUM"
            settings.SetLocalFunctionName("SUM", "SOMME", true);

            // Applicera inställningarna på arbetsboken
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // Anropa GetLocalFunctionName för att hämta det lokalanpassade namnet
                string localName = settings.GetLocalFunctionName("SUM");
                
                // Visa resultatet
                Console.WriteLine($"Localized function name for 'SUM': {localName}");

                // Använd den lokalanpassade funktionen i en cell
                worksheet.Cells["A1"].Formula = "=SOMME(B1:B5)";
                worksheet.Cells["B1"].PutValue(1);
                worksheet.Cells["B2"].PutValue(2);
                worksheet.Cells["B3"].PutValue(3);
                worksheet.Cells["B4"].PutValue(4);
                worksheet.Cells["B5"].PutValue(5);

                // Beräkna formler
                workbook.CalculateFormula();

                // Visa resultatet
                Console.WriteLine($"Calculation result with localized function: {worksheet.Cells["A1"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetLocalFunctionName method: {ex.Message}");
            }
            
            // Spara arbetsboken
            workbook.Save("MethodGetLocalFunctionNameWithStringDemo.xlsx");
        }
    }
}
```

### Se även

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


