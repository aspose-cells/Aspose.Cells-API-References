---
title: "CustomRenderSettings.GetCellBorderWidth"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CustomRenderSettings‑metod. Anger cellkantbredd enligt kanttyp"
type: docs
url: /sv/net/aspose.cells.rendering/customrendersettings/getcellborderwidth/
---
## CustomRenderSettings.GetCellBorderWidth method

Anger cellens kantbredd enligt kanttyp.

```csharp
public virtual float GetCellBorderWidth(CellBorderType borderType)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| borderType | CellBorderType | cellkanttyp |

### Returvärde

cellkantbredd

### Anmärkningar

Alla negativa värden kommer att ignoreras.

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite data för sammanhang
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Skapa en instans av CustomRenderSettings
                CustomRenderSettings renderSettings = new CustomRenderSettings();

                // Anropa GetCellBorderWidth med olika kanttyper
                float thinBorderWidth = renderSettings.GetCellBorderWidth(CellBorderType.Thin);
                float thickBorderWidth = renderSettings.GetCellBorderWidth(CellBorderType.Thick);
                float dashedBorderWidth = renderSettings.GetCellBorderWidth(CellBorderType.Dashed);

                // Visa resultaten
                Console.WriteLine($"Thin border width: {thinBorderWidth}");
                Console.WriteLine($"Thick border width: {thickBorderWidth}");
                Console.WriteLine($"Dashed border width: {dashedBorderWidth}");

                // Spara arbetsboken
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

### Se även

* enum [CellBorderType](../../../aspose.cells/cellbordertype/)
* class [CustomRenderSettings](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


