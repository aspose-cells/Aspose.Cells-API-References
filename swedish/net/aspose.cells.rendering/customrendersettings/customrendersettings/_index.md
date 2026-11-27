---
title: "CustomRenderSettings.CustomRenderSettings"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CustomRenderSettings‑konstruktor. Ctor"
type: docs
url: /sv/net/aspose.cells.rendering/customrendersettings/customrendersettings/
---
## CustomRenderSettings constructor

Konstruktor.

```csharp
public CustomRenderSettings()
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite data för sammanhang
            worksheet.Cells["A1"].Value = "Custom Render Settings Demo";

            try
            {
                // Skapa en instans av CustomRenderSettings med hjälp av konstruktorn
                CustomRenderSettings renderSettings = new CustomRenderSettings();

                // Visa bekräftelse på lyckat anrop av konstruktorn
                Console.WriteLine("CustomRenderSettings instance created successfully using #ctor");

                // Demonstrera att instansen fungerar genom att anropa en metod
                float borderWidth = renderSettings.GetCellBorderWidth(CellBorderType.Thin);
                Console.WriteLine($"Default thin border width: {borderWidth}");

                // Spara arbetsboken
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

### Se även

* class [CustomRenderSettings](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


