---
title: "SettableChartGlobalizationSettings.GetAxisTitleName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SettableChartGlobalizationSettings-Methode. Gibt den Namen des Titels für die Achse zurück"
type: docs
url: /de/net/aspose.cells/settablechartglobalizationsettings/getaxistitlename/
---
## SettableChartGlobalizationSettings.GetAxisTitleName method

Liefert den Namen des Titels für die Achse.

```csharp
public override string GetAxisTitleName()
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableChartGlobalizationSettingsMethodGetAxisTitleNameDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie minimale Daten für den Kontext hinzu
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["A3"].PutValue("Item 2");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);

            try
            {
                // Erstelle eine Instanz von SettableChartGlobalizationSettings
                SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

                // Legen Sie einen benutzerdefinierten Achsentitel fest
                settings.SetAxisTitleName("Custom Axis Title");

                // Rufen Sie den Achsentitelnamen mit GetAxisTitleName ab
                string axisTitleName = settings.GetAxisTitleName();
                Console.WriteLine("Axis Title Name: " + axisTitleName);

                // Speichere die Arbeitsmappe
                workbook.Save("GetAxisTitleNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetAxisTitleName: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


