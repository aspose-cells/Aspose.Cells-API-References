---
title: "SettableGlobalizationSettings.SetLocalFunctionName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SettableGlobalizationSettings-Methode. Legt den lokalisierungsabhängigen Funktionsnamen fest, der dem angegebenen Standardfunktionsnamen entspricht."
type: docs
url: /de/net/aspose.cells/settableglobalizationsettings/setlocalfunctionname/
---
## SettableGlobalizationSettings.SetLocalFunctionName method

Legt den lokalisierungsabhängigen Funktionsnamen fest, der dem angegebenen Standardfunktionsnamen entspricht.

```csharp
public void SetLocalFunctionName(string standardName, string localName, bool bidirectional)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| standardName | String | Standardfunktion (en-US Gebietsschema). |
| localName | String | Lokalisierungsabhängiger Funktionsname |
| bidirectional | Boolean | Ob der lokale Funktionsname automatisch dem Standardfunktionsnamen zugeordnet wird. Wenn true, wird der lokale Name automatisch dem Standardnamen zugeordnet, sodass der Benutzer nicht erneut [`SetStandardFunctionName`](../setstandardfunctionname/) für dasselbe Standard‑ und lokalen Namenspaar aufrufen muss. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetLocalFunctionNameWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstellen Sie Globalisierungseinstellungen
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            try
            {
                // Rufen Sie SetLocalFunctionName auf, um den Standardfunktionsnamen dem lokalen Namen zuzuordnen
                settings.SetLocalFunctionName("SUM", "SOMMA", true); // Italian localization for SUM function
                settings.SetLocalFunctionName("AVERAGE", "MEDIA", true); // Italian localization for AVERAGE function

                // Wenden Sie die Einstellungen auf die Arbeitsmappe an
                workbook.Settings.GlobalizationSettings = settings;

                // Erstellen Sie Formeln, die sowohl Standard‑ als auch lokalisierte Namen verwenden
                worksheet.Cells["A1"].Formula = "=SUM(B1:B5)";
                worksheet.Cells["A2"].Formula = "=SOMMA(B1:B5)";
                worksheet.Cells["A3"].Formula = "=AVERAGE(B1:B5)";
                worksheet.Cells["A4"].Formula = "=MEDIA(B1:B5)";

                // Formeln berechnen
                workbook.CalculateFormula();

                Console.WriteLine("SetLocalFunctionName executed successfully with parameters (String, String, Boolean)");
                Console.WriteLine("Standard and localized function names work equivalently in formulas.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetLocalFunctionName method: {ex.Message}");
            }

            // Ergebnis speichern
            workbook.Save("MethodSetLocalFunctionNameWithStringStringBooleanDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


