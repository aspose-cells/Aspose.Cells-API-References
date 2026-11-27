---
title: "SettableGlobalizationSettings.SetListSeparator"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettableGlobalizationSettings-metoden. Anger avgränsaren för listparametrar i funktion ...etc"
type: docs
url: /sv/net/aspose.cells/settableglobalizationsettings/setlistseparator/
---
## SettableGlobalizationSettings.SetListSeparator method

Ställer in separatorn för list, parameters of function, ...etc.

```csharp
public void SetListSeparator(char c)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| c | Char | den angivna avgränsaren |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetListSeparatorWithCharDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa anpassade globaliseringsinställningar
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            try
            {
                // Anropa SetListSeparator-metoden med en teckenparameter
                settings.SetListSeparator(';');
                
                // Applicera inställningarna på arbetsboken
                workbook.Settings.GlobalizationSettings = settings;
                
                // Visa effekten genom att skapa en formel med listavgränsare
                worksheet.Cells["A1"].Formula = "SUM(1;2;3)";
                worksheet.Cells["A2"].Value = "Formula using custom list separator: SUM(1;2;3)";
                
                Console.WriteLine("SetListSeparator method executed successfully with parameter ';'");
                Console.WriteLine("Formula using custom list separator created in cell A1");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetListSeparator method: {ex.Message}");
            }
            
            // Spara resultatet
            workbook.Save("SetListSeparatorWithCharDemo.xlsx");
        }
    }
}
```

### Se även

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


