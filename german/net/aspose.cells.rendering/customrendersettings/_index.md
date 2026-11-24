---
title: "Klasse CustomRenderSettings"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Rendering.CustomRenderSettings Klasse. Stellt benutzerdefinierte Einstellungen während des Renderns dar"
type: docs
url: /de/net/aspose.cells.rendering/customrendersettings/
---
## CustomRenderSettings class

Stellt benutzerdefinierte Einstellungen während des Renderns dar.

```csharp
public class CustomRenderSettings
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [CustomRenderSettings](customrendersettings/)() | Ctor. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| virtual [GetCellBorderWidth](../../aspose.cells.rendering/customrendersettings/getcellborderwidth/)(CellBorderType) | Gibt die Zellrandbreite gemäß Randtyp an. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingClassCustomRenderSettingsDemo
    {
        public static void Run()
        {
            // Erstellt ein neues Arbeitsbuch für die Demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einige Beispieldaten hinzu
            worksheet.Cells["A1"].Value = "Custom Render Settings Demo";
            worksheet.Cells["A2"].Value = "Border Width Test";

            try
            {
                // Erstellen Sie eine Instanz von CustomRenderSettings mit dem Standardkonstruktor
                CustomRenderSettings renderSettings = new CustomRenderSettings();

                // Demonstrieren Sie die Methode GetCellBorderWidth mit verschiedenen Randtypen
                float thinWidth = renderSettings.GetCellBorderWidth(CellBorderType.Thin);
                float thickWidth = renderSettings.GetCellBorderWidth(CellBorderType.Thick);
                float dashedWidth = renderSettings.GetCellBorderWidth(CellBorderType.Dashed);

                // Ergebnisse anzeigen
                Console.WriteLine($"Thin border width: {thinWidth}");
                Console.WriteLine($"Thick border width: {thickWidth}");
                Console.WriteLine($"Dashed border width: {dashedWidth}");

                // Speichere die Arbeitsmappe
                workbook.Save("CustomRenderSettingsDemo.xlsx");
                Console.WriteLine("CustomRenderSettings demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in CustomRenderSettings demonstration: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


