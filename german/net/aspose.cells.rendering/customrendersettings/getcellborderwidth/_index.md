---
title: "CustomRenderSettings.GetCellBorderWidth"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CustomRenderSettings-Methode. Gibt die Zellrahmenbreite basierend auf dem Rahmentyp an"
type: docs
url: /de/net/aspose.cells.rendering/customrendersettings/getcellborderwidth/
---
## CustomRenderSettings.GetCellBorderWidth method

Gibt die Zellrandbreite gemäß Randtyp an.

```csharp
public virtual float GetCellBorderWidth(CellBorderType borderType)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| borderType | CellBorderType | Zellrahmentyp |

### Rückgabewert

Zellrahmenbreite

### Hinweise

Jeder negative Wert wird ignoriert.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class CustomRenderSettingsMethodGetCellBorderWidthWithCellBorderTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge einige Daten für den Kontext hinzu
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Erstellen Sie eine Instanz von CustomRenderSettings
                CustomRenderSettings renderSettings = new CustomRenderSettings();

                // Rufen Sie GetCellBorderWidth mit verschiedenen Rahmentypen auf
                float thinBorderWidth = renderSettings.GetCellBorderWidth(CellBorderType.Thin);
                float thickBorderWidth = renderSettings.GetCellBorderWidth(CellBorderType.Thick);
                float dashedBorderWidth = renderSettings.GetCellBorderWidth(CellBorderType.Dashed);

                // Ergebnisse anzeigen
                Console.WriteLine($"Thin border width: {thinBorderWidth}");
                Console.WriteLine($"Thick border width: {thickBorderWidth}");
                Console.WriteLine($"Dashed border width: {dashedBorderWidth}");

                // Speichere die Arbeitsmappe
                workbook.Save("GetCellBorderWidthDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* enum [CellBorderType](../../../aspose.cells/cellbordertype/)
* class [CustomRenderSettings](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


