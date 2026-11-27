---
title: "Klass CustomRenderSettings"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Rendering.CustomRenderSettings-klass. Representerar anpassade inställningar under rendering"
type: docs
url: /sv/net/aspose.cells.rendering/customrendersettings/
---
## CustomRenderSettings class

Representerar anpassade inställningar under rendering.

```csharp
public class CustomRenderSettings
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [CustomRenderSettings](customrendersettings/)() | Konstruktor. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| virtual [GetCellBorderWidth](../../aspose.cells.rendering/customrendersettings/getcellborderwidth/)(CellBorderType) | Anger cellens kantbredd enligt kanttyp. |

### Exempel

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
            // Skapa en ny arbetsbok för demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata
            worksheet.Cells["A1"].Value = "Custom Render Settings Demo";
            worksheet.Cells["A2"].Value = "Border Width Test";

            try
            {
                // Skapa en instans av CustomRenderSettings med standardkonstruktorn
                CustomRenderSettings renderSettings = new CustomRenderSettings();

                // Demonstrera GetCellBorderWidth-metoden med olika kanttyper
                float thinWidth = renderSettings.GetCellBorderWidth(CellBorderType.Thin);
                float thickWidth = renderSettings.GetCellBorderWidth(CellBorderType.Thick);
                float dashedWidth = renderSettings.GetCellBorderWidth(CellBorderType.Dashed);

                // Visa resultaten
                Console.WriteLine($"Thin border width: {thinWidth}");
                Console.WriteLine($"Thick border width: {thickWidth}");
                Console.WriteLine($"Dashed border width: {dashedWidth}");

                // Spara arbetsboken
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

### Se även

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


