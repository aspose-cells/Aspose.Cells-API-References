---
title: "SettableGlobalizationSettings.SetListSeparator"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SettableGlobalizationSettings-Methode. Legt das Trennzeichen für Listenparameter einer Funktion fest …usw."
type: docs
url: /de/net/aspose.cells/settableglobalizationsettings/setlistseparator/
---
## SettableGlobalizationSettings.SetListSeparator method

Legt das Trennzeichen für Listen, Funktionsparameter, … usw. fest.

```csharp
public void SetListSeparator(char c)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| c | Char | der angegebene Trenner |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetListSeparatorWithCharDemo
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
                // Rufen Sie die SetListSeparator‑Methode mit einem Zeichenparameter auf
                settings.SetListSeparator(';');
                
                // Wenden Sie die Einstellungen auf die Arbeitsmappe an
                workbook.Settings.GlobalizationSettings = settings;
                
                // Demonstrieren Sie die Wirkung, indem Sie eine Formel mit Listentrennzeichen erstellen
                worksheet.Cells["A1"].Formula = "SUM(1;2;3)";
                worksheet.Cells["A2"].Value = "Formula using custom list separator: SUM(1;2;3)";
                
                Console.WriteLine("SetListSeparator method executed successfully with parameter ';'");
                Console.WriteLine("Formula using custom list separator created in cell A1");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetListSeparator method: {ex.Message}");
            }
            
            // Ergebnis speichern
            workbook.Save("SetListSeparatorWithCharDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


