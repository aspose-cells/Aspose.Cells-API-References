---
title: "SettableChartGlobalizationSettings.SetOtherName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SettableChartGlobalizationSettings-Methode. Legt den Namen der anderen Beschriftungen für das Diagramm fest"
type: docs
url: /de/net/aspose.cells/settablechartglobalizationsettings/setothername/
---
## SettableChartGlobalizationSettings.SetOtherName method

Setzt den Namen der "Other"-Beschriftungen für das Diagramm.

```csharp
public void SetOtherName(string name)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | String | lokaler abhängiger Name |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableChartGlobalizationSettingsMethodSetOtherNameWithStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie minimale Daten für den Kontext hinzu
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(150);

            try
            {
                // Erstelle eine Instanz von SettableChartGlobalizationSettings
                SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

                // Setze einen benutzerdefinierten Namen für die "Other"-Beschriftung.
                settings.SetOtherName("Miscellaneous Items");

                // Überprüfen Sie die Einstellung, indem Sie den Wert abrufen
                string otherName = settings.GetOtherName();
                Console.WriteLine("Other Name set to: " + otherName);

                // Speichere die Arbeitsmappe
                workbook.Save("SetOtherNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetOtherName: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


