---
title: "SettableGlobalizationSettings.GetBooleanValueString"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettableGlobalizationSettings-metoden. Hämtar displaysträngvärdet för cellers booleska värde"
type: docs
url: /sv/net/aspose.cells/settableglobalizationsettings/getbooleanvaluestring/
---
## SettableGlobalizationSettings.GetBooleanValueString method

Hämtar visningssträngvärdet för cellens booleska värde

```csharp
public override string GetBooleanValueString(bool bv)
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

    public class SettableGlobalizationSettingsMethodGetBooleanValueStringWithBooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa anpassade globaliseringsinställningar
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // Ange anpassade booleska värdesträngar
            settings.SetBooleanValueString(true, "TRUE_CUSTOM");
            settings.SetBooleanValueString(false, "FALSE_CUSTOM");

            // Applicera inställningarna på arbetsboken
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // Anropa GetBooleanValueString med true
                string trueValue = settings.GetBooleanValueString(true);
                Console.WriteLine("Custom true value: " + trueValue);

                // Anropa GetBooleanValueString med false
                string falseValue = settings.GetBooleanValueString(false);
                Console.WriteLine("Custom false value: " + falseValue);

                // Visa effekten i kalkylbladet
                worksheet.Cells["A1"].PutValue(true);
                worksheet.Cells["A2"].PutValue(false);

                Console.WriteLine("Cell A1 value: " + worksheet.Cells["A1"].StringValue);
                Console.WriteLine("Cell A2 value: " + worksheet.Cells["A2"].StringValue);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetBooleanValueString method: {ex.Message}");
            }

            // Spara arbetsboken
            workbook.Save("SettableGlobalizationSettingsMethodGetBooleanValueStringDemo.xlsx");
        }
    }
}
```

### Se även

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


