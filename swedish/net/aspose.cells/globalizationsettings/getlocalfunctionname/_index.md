---
title: "GlobalizationSettings.GetLocalFunctionName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GlobalizationSettings-metoden. Hämtar den lokalanpassade funktionsnamnet enligt angivet standardfunktionsnamn"
type: docs
url: /sv/net/aspose.cells/globalizationsettings/getlocalfunctionname/
---
## GlobalizationSettings.GetLocalFunctionName method

Hämtar det lokalanpassade funktionsnamnet enligt given standardfunktionsnamn.

```csharp
public virtual string GetLocalFunctionName(string standardName)
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

    public class GlobalizationSettingsMethodGetLocalFunctionNameWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ställ in anpassade globaliseringsinställningar
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            // Lägg till exempeldata
            worksheet.Cells["B1"].PutValue(5);
            worksheet.Cells["B2"].PutValue(15);

            // Skapa formel med lokalanpassat funktionsnamn
            Cell cell = worksheet.Cells["B3"];
            cell.Formula = "=LOCALSUM(B1:B2)";

            try
            {
                workbook.CalculateFormula();
                Console.WriteLine($"Calculation result using localized function: {cell.DoubleValue}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Calculation error: {ex.Message}");
            }

            workbook.Save("GlobalizationSettingsFunctionDemo.xlsx");
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override string GetLocalFunctionName(string standardName)
            {
                if (standardName == "SUM")
                {
                    return "LOCALSUM";
                }
                return base.GetLocalFunctionName(standardName);
            }
        }
    }
}
```

### Se även

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


