---
title: "SettableGlobalizationSettings.SetStandardFunctionName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SettableGlobalizationSettings‑Methode. Setzt den lokalisierungsabhängigen Funktionsnamen gemäß dem angegebenen Standardfunktionsnamen."
type: docs
url: /de/net/aspose.cells/settableglobalizationsettings/setstandardfunctionname/
---
## SettableGlobalizationSettings.SetStandardFunctionName method

Legt den lokalisierungsabhängigen Funktionsnamen gemäß dem angegebenen Standardfunktionsnamen fest.

```csharp
public void SetStandardFunctionName(string localName, string standardName, bool bidirectional)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| localName | String | Lokalisierungsabhängiger Funktionsname |
| standardName | String | Standardfunktion (en-US Gebietsschema). |
| bidirectional | Boolean | Ob der Standardfunktionsname automatisch auf den lokalen Funktionsnamen abgebildet wird. Wenn true, wird der Standardname automatisch auf den lokalen Namen abgebildet, sodass der Benutzer nicht erneut [`SetLocalFunctionName`](../setlocalfunctionname/) für dasselbe Standard‑ und Lokalpaar aufrufen muss. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetStandardFunctionNameWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle benutzerdefinierte Globalisierungseinstellungen
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            try
            {
                // Rufen Sie SetStandardFunctionName auf, um einen lokalen Funktionsnamen auf den Standardnamen abzubilden.
                settings.SetStandardFunctionName("LOCAL_SUM", "SUM", true);

                // Wenden Sie die Einstellungen auf die Arbeitsmappe an.
                workbook.Settings.GlobalizationSettings = settings;

                // Erstellen Sie eine Formel mit dem lokalen Funktionsnamen
                worksheet.Cells["A1"].Formula = "=LOCAL_SUM(B1:B3)";
                worksheet.Cells["B1"].Value = 10;
                worksheet.Cells["B2"].Value = 20;
                worksheet.Cells["B3"].Value = 30;

                // Formel berechnen
                workbook.CalculateFormula();

                Console.WriteLine("Formula with local function name 'LOCAL_SUM' calculated successfully.");
                Console.WriteLine($"Result: {worksheet.Cells["A1"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetStandardFunctionName method: {ex.Message}");
            }

            // Ergebnis speichern
            workbook.Save("SetStandardFunctionNameDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


