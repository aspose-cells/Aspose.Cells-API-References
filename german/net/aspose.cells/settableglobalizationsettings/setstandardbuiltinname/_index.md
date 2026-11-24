---
title: "SettableGlobalizationSettings.SetStandardBuiltInName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SettableGlobalizationSettings‑Methode. Setzt den lokalisierungsabhängigen Funktionsnamen gemäß dem angegebenen Standardfunktionsnamen."
type: docs
url: /de/net/aspose.cells/settableglobalizationsettings/setstandardbuiltinname/
---
## SettableGlobalizationSettings.SetStandardBuiltInName method

Legt den lokalisierungsabhängigen Funktionsnamen gemäß dem angegebenen Standardfunktionsnamen fest.

```csharp
public void SetStandardBuiltInName(string localName, string standardName, bool bidirectional)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| localName | String | Lokalisierungsabhängiger Funktionsname |
| standardName | String | Standardfunktion (en-US Gebietsschema). |
| bidirectional | Boolean | Ob der Standard-Namens-Text automatisch auf den lokalen Namens-Text abgebildet wird. Wenn true, wird der Standard-Namens-Text automatisch auf den lokalen Namens-Text abgebildet, sodass der Benutzer nicht erneut [`SetLocalBuiltInName`](../setlocalbuiltinname/) für dasselbe Standard- und lokale Namenspaar aufrufen muss. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetStandardBuiltInNameWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Erstelle benutzerdefinierte Globalisierungseinstellungen
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // Legen Sie die Globalisierungseinstellungen für die Arbeitsmappe fest
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // Rufen Sie SetStandardBuiltInName auf, um einen lokalen Namen auf einen standardmäßigen integrierten Namen abzubilden
                // Parameter: localName, standardName, bidirectional
                settings.SetStandardBuiltInName("MyLocalName", "SUM", true);
                
                Console.WriteLine("SetStandardBuiltInName executed successfully with parameters (\"MyLocalName\", \"SUM\", true)");
                
                // Demonstrieren Sie die Wirkung, indem Sie den lokalen Namen in einer Formel verwenden
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].PutValue(10);
                worksheet.Cells["A2"].PutValue(20);
                worksheet.Cells["A3"].Formula = "=MyLocalName(A1:A2)";
                
                // Berechnen Sie die Formel, um zu zeigen, dass sie mit dem lokalen Namen funktioniert
                workbook.CalculateFormula();
                Console.WriteLine("Result of formula with local name: " + worksheet.Cells["A3"].Value);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetStandardBuiltInName method: {ex.Message}");
            }
            
            // Ergebnis speichern
            workbook.Save("SetStandardBuiltInNameDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


