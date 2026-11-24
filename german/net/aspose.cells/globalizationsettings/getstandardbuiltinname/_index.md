---
title: "GlobalizationSettings.GetStandardBuiltInName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GlobalizationSettings-Methode. Gibt den Standardtext des integrierten Namens gemäß dem lokalisierungsabhängigen Text zurück"
type: docs
url: /de/net/aspose.cells/globalizationsettings/getstandardbuiltinname/
---
## GlobalizationSettings.GetStandardBuiltInName method

Gibt den Standardtext des integrierten Namens gemäß dem gegebenen lokalisierungsabhängigen Text zurück.

```csharp
public virtual string GetStandardBuiltInName(string localName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| localName | String | Lokalisierungsabhängiger Text des integrierten Namens. Das Gebietsschema wurde vom Arbeitsbuch angegeben, für das diese Einstellung verwendet wird. |

### Rückgabewert

Standardtext (en-US‑Gebietsschema).

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsMethodGetStandardBuiltInNameWithStringDemo
    {
        public static void Run()
        {
            // Arbeitsmappe mit benutzerdefinierten Globalisierungseinstellungen erstellen
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Benutzerdefinierte Globalisierungseinstellungen initialisieren und der Arbeitsmappe zuweisen
            var globalizationSettings = new CustomGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = globalizationSettings;

            // Parameter für GetStandardBuiltInName testen
            string localFunctionName = "MyLocalSum";
            
            try
            {
                // Rufe GetStandardBuiltInName mit lokalem Funktionsnamen auf
                string standardName = globalizationSettings.GetStandardBuiltInName(localFunctionName);
                Console.WriteLine($"Local name: '{localFunctionName}' => Standard name: '{standardName}'");

                // Demonstriere die Wirkung, indem du den lokalen Namen in einer Formel verwendest
                worksheet.Cells["A1"].Value = 5;
                worksheet.Cells["A2"].Value = 7;
                worksheet.Cells["A3"].Formula = $"{localFunctionName}(A1:A2)";

                // Formel berechnen, um die korrekte Interpretation anzuzeigen
                workbook.CalculateFormula();
                Console.WriteLine($"Formula result: {worksheet.Cells["A3"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetStandardBuiltInName: {ex.Message}");
            }

            // Speichere die geänderte Arbeitsmappe
            workbook.Save("GlobalizationGetStandardBuiltInNameDemo.xlsx");
        }
    }

    // Benutzerdefinierte Globalisierungseinstellungen überschreiben GetStandardBuiltInName
    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetStandardBuiltInName(string localName)
        {
            // Ordne benutzerdefinierten lokalen Funktionsnamen dem Standard‑SUM zu
            if (localName.Equals("MyLocalSum", StringComparison.OrdinalIgnoreCase))
            {
                return "SUM";
            }
            return base.GetStandardBuiltInName(localName);
        }
    }
}
```

### Siehe auch

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


