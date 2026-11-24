---
title: "CustomRenderSettings.CustomRenderSettings"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CustomRenderSettings-Konstruktor. Ctor"
type: docs
url: /de/net/aspose.cells.rendering/customrendersettings/customrendersettings/
---
## CustomRenderSettings constructor

Ctor.

```csharp
public CustomRenderSettings()
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class CustomRenderSettingsMethodSharpctorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge einige Daten für den Kontext hinzu
            worksheet.Cells["A1"].Value = "Custom Render Settings Demo";

            try
            {
                // Erstellen Sie eine Instanz von CustomRenderSettings mit dem Konstruktor
                CustomRenderSettings renderSettings = new CustomRenderSettings();

                // Anzeige der Bestätigung des erfolgreichen Aufrufs des Konstruktors
                Console.WriteLine("CustomRenderSettings instance created successfully using #ctor");

                // Demonstrieren Sie, dass die Instanz funktionsfähig ist, indem Sie eine Methode aufrufen
                float borderWidth = renderSettings.GetCellBorderWidth(CellBorderType.Thin);
                Console.WriteLine($"Default thin border width: {borderWidth}");

                // Speichere die Arbeitsmappe
                workbook.Save("CustomRenderSettingsDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating CustomRenderSettings: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [CustomRenderSettings](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


