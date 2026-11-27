---
title: "GlobalizationSettings.GetBooleanValueString"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GlobalizationSettings-metoden. Hämtar displaysträngvärdet för cellers booleska värde"
type: docs
url: /sv/net/aspose.cells/globalizationsettings/getbooleanvaluestring/
---
## GlobalizationSettings.GetBooleanValueString method

Hämtar visningssträngvärdet för cellens booleska värde

```csharp
public virtual string GetBooleanValueString(bool bv)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| bv | Boolean | booleskt värde |

### Returvärde

Returnerar som standard "TRUE" för sant värde och "FALSE" för falskt värde.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsMethodGetBooleanValueStringWithBooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med anpassade globaliseringsinställningar
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = new CustomBooleanGlobalizationSettings();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Demonstrera GetBooleanValueString med båda booleska värdena
                var globalizationSettings = workbook.Settings.GlobalizationSettings;
                string trueResult = globalizationSettings.GetBooleanValueString(true);
                string falseResult = globalizationSettings.GetBooleanValueString(false);

                Console.WriteLine($"GetBooleanValueString(true) returns: {trueResult}");
                Console.WriteLine($"GetBooleanValueString(false) returns: {falseResult}");

                // Applicera booleska värden på celler för att visa kalkylblads-effekt
                worksheet.Cells["A1"].PutValue(true);
                worksheet.Cells["A2"].PutValue(false);

                workbook.Save("GlobalizationBooleanDemo.xlsx");
                Console.WriteLine("Workbook saved with custom boolean representations.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetBooleanValueString: {ex.Message}");
            }
        }
    }

    // Anpassade globaliseringsinställningar som åsidosätter boolesk strängrepresentation
    public class CustomBooleanGlobalizationSettings : GlobalizationSettings
    {
        public override string GetBooleanValueString(bool bv)
        {
            return bv ? "Enabled" : "Disabled";
        }
    }
}
```

### Se även

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


