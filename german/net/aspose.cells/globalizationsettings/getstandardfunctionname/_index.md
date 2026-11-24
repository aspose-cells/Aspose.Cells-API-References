---
title: "GlobalizationSettings.GetStandardFunctionName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GlobalizationSettings‑Methode. Gibt den Standardfunktionsnamen basierend auf dem angegebenen lokalisierungsabhängigen Funktionsnamen zurück"
type: docs
url: /de/net/aspose.cells/globalizationsettings/getstandardfunctionname/
---
## GlobalizationSettings.GetStandardFunctionName method

Gibt den Standardfunktionsnamen gemäß dem gegebenen lokalisierungsabhängigen Funktionsnamen zurück.

```csharp
public virtual string GetStandardFunctionName(string localName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| localName | String | Lokalisierungsabhängiger Funktionsname. Das Gebietsschema wurde vom Arbeitsbuch angegeben, für das diese Einstellung verwendet wird. |

### Rückgabewert

Standardfunktion (en-US Gebietsschema).

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsMethodGetStandardFunctionNameWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten vorbereiten
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["A2"].PutValue(15);
            
            // Erstellen Sie benutzerdefinierte Globalisierungseinstellungen und weisen Sie sie dem Arbeitsbuch zu
            var customSettings = new CustomGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = customSettings;

            try
            {
                // Demonstriert GetStandardFunctionName mit dem deutschen SUM-Funktionsnamen
                string localName = "SUMME";
                string standardName = customSettings.GetStandardFunctionName(localName);
                
                Console.WriteLine($"Local function name: {localName}");
                Console.WriteLine($"Standard function name: {standardName}");

                // Lokalen Funktionsnamen in der Formel anwenden
                worksheet.Cells["A3"].Formula = "=SUMME(A1:A2)";
                workbook.CalculateFormula();
                
                Console.WriteLine($"Formula result: {worksheet.Cells["A3"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetStandardFunctionName method: {ex.Message}");
            }

            workbook.Save("MethodGetStandardFunctionNameDemo.xlsx");
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override string GetStandardFunctionName(string localName)
            {
                // Deutschen Funktionsnamen in standardmäßiges Englisch konvertieren
                if (localName.Equals("SUMME", StringComparison.OrdinalIgnoreCase))
                {
                    return "SUM";
                }
                return base.GetStandardFunctionName(localName);
            }
        }
    }
}
```

### Siehe auch

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


