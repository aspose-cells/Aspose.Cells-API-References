---
title: "SettableGlobalizationSettings.GetStandardFunctionName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SettableGlobalizationSettings-Methode. Gibt den Standardfunktionsnamen gemäß dem angegebenen lokalisierungsabhängigen Funktionsnamen zurück."
type: docs
url: /de/net/aspose.cells/settableglobalizationsettings/getstandardfunctionname/
---
## SettableGlobalizationSettings.GetStandardFunctionName method

Gibt den Standardfunktionsnamen gemäß dem gegebenen lokalisierungsabhängigen Funktionsnamen zurück.

```csharp
public override string GetStandardFunctionName(string localName)
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

    public class SettableGlobalizationSettingsMethodGetStandardFunctionNameWithStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle benutzerdefinierte Globalisierungseinstellungen
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // Lokale Funktionsnamenzuordnung festlegen
            settings.SetStandardFunctionName("LocalSum", "SUM", true);

            // Wenden Sie die Einstellungen auf die Arbeitsmappe an
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // Rufen Sie GetStandardFunctionName mit einem lokalen Funktionsnamen auf
                string standardName = settings.GetStandardFunctionName("LocalSum");
                
                // Ergebnis anzeigen
                Console.WriteLine($"Standard function name for 'LocalSum' is: {standardName}");

                // Verwenden Sie die Standardfunktion in einer Zellformel
                worksheet.Cells["A1"].Formula = $"={standardName}(1,2,3)";
                worksheet.Cells["A2"].Value = 1;
                worksheet.Cells["A3"].Value = 2;
                worksheet.Cells["A4"].Value = 3;

                // Formel berechnen
                workbook.CalculateFormula();

                // Ergebnis anzeigen
                Console.WriteLine($"Formula result in A1: {worksheet.Cells["A1"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetStandardFunctionName method: {ex.Message}");
            }
            
            // Speichere die Arbeitsmappe
            workbook.Save("SettableGlobalizationSettingsMethodGetStandardFunctionNameWithStringDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


