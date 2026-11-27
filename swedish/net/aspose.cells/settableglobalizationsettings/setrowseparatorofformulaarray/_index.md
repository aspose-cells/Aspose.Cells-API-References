---
title: "SettableGlobalizationSettings.SetRowSeparatorOfFormulaArray"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettableGlobalizationSettings-metoden. Anger avgränsaren för rader i matrisdata i formeln"
type: docs
url: /sv/net/aspose.cells/settableglobalizationsettings/setrowseparatorofformulaarray/
---
## SettableGlobalizationSettings.SetRowSeparatorOfFormulaArray method

Ställer in separatorn för rader i array data i formeln.

```csharp
public void SetRowSeparatorOfFormulaArray(char c)
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

    public class SettableGlobalizationSettingsMethodSetRowSeparatorOfFormulaArrayDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa anpassade globaliseringsinställningar
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // Ställ in radavgränsaren för formelmatriser till '|'
            char rowSeparator = '|';
            settings.SetRowSeparatorOfFormulaArray(rowSeparator);

            // Applicera inställningarna på arbetsboken
            workbook.Settings.GlobalizationSettings = settings;

            // Skapa en matrisformel i kalkylbladet
            worksheet.Cells["A1"].SetArrayFormula("={1,2,3;4,5,6}", 2, 3);
            
            try
            {
                // Beräkna formeln för att tillämpa inställningarna
                workbook.CalculateFormula();

                // Visa formeln med den nya radavgränsaren
                Console.WriteLine("Array formula with custom row separator: " + worksheet.Cells["A1"].Formula);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetRowSeparatorOfFormulaArray method: {ex.Message}");
            }
            
            // Spara arbetsboken
            workbook.Save("MethodSetRowSeparatorOfFormulaArrayDemo.xlsx");
        }
    }
}
```

### Se även

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


