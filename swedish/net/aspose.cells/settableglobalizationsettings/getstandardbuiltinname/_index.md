---
title: "SettableGlobalizationSettings.GetStandardBuiltInName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettableGlobalizationSettings-metoden. Hämtar standardtexten för inbyggt namn enligt given localespecifik text"
type: docs
url: /sv/net/aspose.cells/settableglobalizationsettings/getstandardbuiltinname/
---
## SettableGlobalizationSettings.GetStandardBuiltInName method

Hämtar standardtexten för inbyggt namn enligt given lokalanpassad text.

```csharp
public override string GetStandardBuiltInName(string localName)
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

    public class SettableGlobalizationSettingsMethodGetStandardBuiltInNameWithStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en instans av SettableGlobalizationSettings
            SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();

            // Ange ett lokalt inbyggt namn för demonstration
            globalizationSettings.SetLocalBuiltInName("SUM", "LocalSumName", true);

            try
            {
                // Anropa GetStandardBuiltInName-metoden med ett lokalt namn
                string standardName = globalizationSettings.GetStandardBuiltInName("LocalSumName");
                
                // Visa resultatet
                Console.WriteLine($"Standard name for 'LocalSumName' is: {standardName}");

                // Tillämpa resultatet på en cell
                worksheet.Cells["A1"].Formula = "=" + standardName + "(1,2,3)";
                workbook.CalculateFormula();

                // Visa det beräknade resultatet
                Console.WriteLine($"Result of formula in A1: {worksheet.Cells["A1"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetStandardBuiltInName method: {ex.Message}");
            }
            
            // Spara arbetsboken
            workbook.Save("SettableGlobalizationSettingsMethodGetStandardBuiltInNameWithStringDemo.xlsx");
        }
    }
}
```

### Se även

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


