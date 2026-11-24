---
title: "SettableGlobalizationSettings.GetLocalFunctionName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SettableGlobalizationSettings‑Methode. Gibt den lokalisierungsabhängigen Funktionsnamen gemäß dem angegebenen Standardfunktionsnamen zurück"
type: docs
url: /de/net/aspose.cells/settableglobalizationsettings/getlocalfunctionname/
---
## SettableGlobalizationSettings.GetLocalFunctionName method

Gibt den lokalisierungsabhängigen Funktionsnamen gemäß dem angegebenen Standardfunktionsnamen zurück.

```csharp
public override string GetLocalFunctionName(string standardName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| standardName | String | Standardfunktion (en-US Gebietsschema). |

### Rückgabewert

Lokalisierungsabhängiger Funktionsname. Das Gebietsschema wurde vom Arbeitsbuch angegeben, für das diese Einstellung verwendet wird.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodGetLocalFunctionNameWithStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle benutzerdefinierte Globalisierungseinstellungen
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // Legen Sie einen benutzerdefinierten lokalen Funktionsnamen für "SUM" fest
            settings.SetLocalFunctionName("SUM", "SOMME", true);

            // Wenden Sie die Einstellungen auf die Arbeitsmappe an
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // Rufen Sie GetLocalFunctionName auf, um den lokalisierten Namen abzurufen
                string localName = settings.GetLocalFunctionName("SUM");
                
                // Ergebnis anzeigen
                Console.WriteLine($"Localized function name for 'SUM': {localName}");

                // Verwenden Sie die lokalisierte Funktion in einer Zelle
                worksheet.Cells["A1"].Formula = "=SOMME(B1:B5)";
                worksheet.Cells["B1"].PutValue(1);
                worksheet.Cells["B2"].PutValue(2);
                worksheet.Cells["B3"].PutValue(3);
                worksheet.Cells["B4"].PutValue(4);
                worksheet.Cells["B5"].PutValue(5);

                // Formeln berechnen
                workbook.CalculateFormula();

                // Ergebnis anzeigen
                Console.WriteLine($"Calculation result with localized function: {worksheet.Cells["A1"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetLocalFunctionName method: {ex.Message}");
            }
            
            // Speichere die Arbeitsmappe
            workbook.Save("MethodGetLocalFunctionNameWithStringDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


