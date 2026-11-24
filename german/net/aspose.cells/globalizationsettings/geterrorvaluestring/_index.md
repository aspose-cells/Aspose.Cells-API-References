---
title: "GlobalizationSettings.GetErrorValueString"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GlobalizationSettings-Methode. Gibt den Anzeigetextwert für den Fehlwert einer Zelle zurück"
type: docs
url: /de/net/aspose.cells/globalizationsettings/geterrorvaluestring/
---
## GlobalizationSettings.GetErrorValueString method

Gibt den Anzeigestringwert für den Fehlerwert einer Zelle zurück.

```csharp
public virtual string GetErrorValueString(string err)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| err | String | Fehlerwerte wie #VALUE!, #NAME? |

### Rückgabewert

Gibt standardmäßig den Fehlwert selbst zurück

### Beispiele

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
            
            // Benutzerdefinierte Globalisierungseinstellungen festlegen
            workbook.Settings.GlobalizationSettings = new CustomErrorGlobalizationSettings();

            // Fehlerfall erstellen: Division durch Null
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
            // Benutzerdefinierte Zuordnungen von Fehlwerten
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

### Siehe auch

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


