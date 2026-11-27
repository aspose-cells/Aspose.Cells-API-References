---
title: "GlobalizationSettings.GetErrorValueString"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GlobalizationSettings-metoden. Hämtar visningssträngvärdet för cellers felvärde"
type: docs
url: /sv/net/aspose.cells/globalizationsettings/geterrorvaluestring/
---
## GlobalizationSettings.GetErrorValueString method

Hämtar visningssträngvärdet för cellens felvärde

```csharp
public virtual string GetErrorValueString(string err)
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

    public class GlobalizationSettingsMethodGetErrorValueStringWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ställ in anpassade globaliseringsinställningar
            workbook.Settings.GlobalizationSettings = new CustomErrorGlobalizationSettings();

            // Skapa felscenario: Division med noll
            Cell cell = worksheet.Cells["A1"];
            cell.Formula = "=1/0";  // This will generate #DIV/0! error

            try
            {
                workbook.CalculateFormula();
                string errorValue = cell.DisplayStringValue;
                
                Console.WriteLine($"Error display value: {errorValue}");
                Console.WriteLine("Method executed successfully - see custom error mapping");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetErrorValueString method: {ex.Message}");
            }

            workbook.Save("MethodGetErrorValueStringDemo.xlsx");
        }
    }

    public class CustomErrorGlobalizationSettings : GlobalizationSettings
    {
        public override string GetErrorValueString(string err)
        {
            // Anpassade felvärdemappningar
            return err switch
            {
                "#DIV/0!" => "Custom Division Error",
                "#VALUE!" => "Custom Type Mismatch",
                "#NAME?" => "Custom Identifier Error",
                _ => base.GetErrorValueString(err)
            };
        }
    }
}
```

### Se även

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


