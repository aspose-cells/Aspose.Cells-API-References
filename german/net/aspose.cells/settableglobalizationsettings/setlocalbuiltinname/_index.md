---
title: "SettableGlobalizationSettings.SetLocalBuiltInName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SettableGlobalizationSettings-Methode. Legt den lokalisierungsabhängigen Text für den eingebauten Namen mit dem angegebenen Standardnamen-Text fest"
type: docs
url: /de/net/aspose.cells/settableglobalizationsettings/setlocalbuiltinname/
---
## SettableGlobalizationSettings.SetLocalBuiltInName method

Legt den lokalisierungsabhängigen Text für den integrierten Namen mit dem angegebenen Standardnamen‑Text fest.

```csharp
public void SetLocalBuiltInName(string standardName, string localName, bool bidirectional)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| standardName | String | Standard-(en-US-Locale) Namens-Text des integrierten Namens. |
| localName | String | Lokalisierungsabhängiger Namens-Text |
| bidirectional | Boolean | Ob der lokale Namens-Text automatisch auf den Standard-Namens-Text abgebildet wird. Wenn true, wird der lokale Namens-Text automatisch auf den Standard-Namens-Text abgebildet, sodass der Benutzer nicht erneut [`SetStandardBuiltInName`](../setstandardbuiltinname/) für dasselbe Standard- und lokale Namenspaar aufrufen muss. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetLocalBuiltInNameWithStringStringBooleanDemo
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
                // Rufen Sie SetLocalBuiltInName auf, um einen standardmäßigen integrierten Namen auf einen lokalen Namen abzubilden
                settings.SetLocalBuiltInName("SUM", "LOCAL_SUM", true);

                // Wenden Sie die Einstellungen auf die Arbeitsmappe an
                workbook.Settings.GlobalizationSettings = settings;

                // Erstellen Sie eine Formel mit dem standardmäßigen integrierten Namen
                worksheet.Cells["A1"].Formula = "=SUM(B1:B3)";
                worksheet.Cells["B1"].Value = 5;
                worksheet.Cells["B2"].Value = 10;
                worksheet.Cells["B3"].Value = 15;

                // Formel berechnen
                workbook.CalculateFormula();

                Console.WriteLine("Formula with standard built-in name 'SUM' calculated successfully.");
                Console.WriteLine($"Result: {worksheet.Cells["A1"].Value}");

                // Überprüfen Sie die Zuordnung des lokalen Namens
                string localName = settings.GetLocalBuiltInName("SUM");
                Console.WriteLine($"Local name for 'SUM': {localName}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetLocalBuiltInName method: {ex.Message}");
            }

            // Ergebnis speichern
            workbook.Save("SetLocalBuiltInNameDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


