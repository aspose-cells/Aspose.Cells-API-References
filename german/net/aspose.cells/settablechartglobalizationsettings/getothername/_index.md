---
title: "SettableChartGlobalizationSettings.GetOtherName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SettableChartGlobalizationSettings-Methode. Gibt den Namen der \"Other\"-Beschriftungen für das Diagramm zurück."
type: docs
url: /de/net/aspose.cells/settablechartglobalizationsettings/getothername/
---
## SettableChartGlobalizationSettings.GetOtherName method

Ermittelt den Namen der "Other"-Beschriftungen für das Diagramm.

```csharp
public override string GetOtherName()
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableChartGlobalizationSettingsMethodGetOtherNameDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine neue Arbeitsmappe und rufen Sie das erste Arbeitsblatt ab
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge minimale Daten hinzu (optional, nur für ein vollständiges Workbook).
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["A3"].PutValue("Item 2");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(120);
            worksheet.Cells["B3"].PutValue(250);

            try
            {
                // Instanziiere das Globalisierungs‑Einstellungsobjekt.
                SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

                // Setze einen benutzerdefinierten Namen für die "Other"-Beschriftung.
                settings.SetOtherName("Custom Other Label");

                // Rufe den Namen mit GetOtherName ab.
                string otherName = settings.GetOtherName();

                Console.WriteLine("Other Name retrieved: " + otherName);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetOtherName: {ex.Message}");
            }

            // Speichere das Workbook (die Einstellungen sind in diesem Demo nicht direkt dem Diagramm zugeordnet).
            workbook.Save("GetOtherNameDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


