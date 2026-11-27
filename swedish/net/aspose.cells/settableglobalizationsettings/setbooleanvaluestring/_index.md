---
title: "SettableGlobalizationSettings.SetBooleanValueString"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettableGlobalizationSettings-metoden. Anger visningssträngvärdet för cellernas booleska värde"
type: docs
url: /sv/net/aspose.cells/settableglobalizationsettings/setbooleanvaluestring/
---
## SettableGlobalizationSettings.SetBooleanValueString method

Ställer in visningssträngvärdet för cellens booleska värde

```csharp
public void SetBooleanValueString(bool bv, string name)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| bv | Boolean | booleskt värde |
| namn | String | strängvärde för det booleska värdet |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetBooleanValueStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa anpassade globaliseringsinställningar
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // Ange anpassade booleska värdesträngar
            settings.SetBooleanValueString(true, "Yes");
            settings.SetBooleanValueString(false, "No");
            
            // Applicera inställningarna på arbetsboken
            workbook.Settings.GlobalizationSettings = settings;
            
            // Ange booleska värden i celler
            worksheet.Cells["A1"].PutValue(true);
            worksheet.Cells["A2"].PutValue(false);
            
            // Ställ in visningsstil för att visa booleska värden som text
            Style style = workbook.CreateStyle();
            style.Custom = "BOOLEAN";
            worksheet.Cells["A1"].SetStyle(style);
            worksheet.Cells["A2"].SetStyle(style);
            
            try
            {
                // Spara arbetsboken
                workbook.Save("SetBooleanValueStringDemo.xlsx");
                Console.WriteLine("Workbook saved with custom boolean value strings.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error saving workbook: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


