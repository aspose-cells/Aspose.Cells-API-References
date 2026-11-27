---
title: "SettableGlobalizationSettings.GetErrorValueString"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettableGlobalizationSettings-metoden. Hämtar displaysträngsvärdet för cellers felvärde"
type: docs
url: /sv/net/aspose.cells/settableglobalizationsettings/geterrorvaluestring/
---
## SettableGlobalizationSettings.GetErrorValueString method

Hämtar visningssträngvärdet för cellens felvärde

```csharp
public override string GetErrorValueString(string err)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| err | String | felvärden såsom #VALUE!,#NAME? |

### Returvärde

Returnerar som standard själva felvärdet

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodGetErrorValueStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa anpassade globaliseringsinställningar
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = settings;

            // Skapa en cell med felvärde
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("#N/A");
            Style style = workbook.CreateStyle();
            cell.SetStyle(style);
            style.Number = 10; // Set format to Error value

            try
            {
                // Anropa GetErrorValueString med felvärdessträng
                string errorString = settings.GetErrorValueString("#N/A");
                
                // Visa resultatet
                Console.WriteLine("Error value string: " + errorString);

                // Visa effekten genom att sätta en annan cells värde till den returnerade strängen
                worksheet.Cells["A2"].PutValue("Error representation: " + errorString);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetErrorValueString method: {ex.Message}");
            }
            
            // Spara arbetsboken
            workbook.Save("MethodGetErrorValueStringDemo.xlsx");
        }
    }
}
```

### Se även

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


