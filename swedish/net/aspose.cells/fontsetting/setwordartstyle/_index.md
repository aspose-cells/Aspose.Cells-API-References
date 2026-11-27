---
title: "FontSetting.SetWordArtStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FontSetting-metod. Ställer in den förinställda WordArt-stilen"
type: docs
url: /sv/net/aspose.cells/fontsetting/setwordartstyle/
---
## FontSetting.SetWordArtStyle method

Ställer in den förinställda WordArt-stilen.

```csharp
public void SetWordArtStyle(PresetWordArtStyle style)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| style | PresetWordArtStyle | Den förinställda WordArt-stilen. |

### Anmärkningar

Endast för texten i form/diagram.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class FontSettingMethodSetWordArtStyleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite text i cell A1
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text for WordArt");

            // Skapa teckensnittinställning för texten i cell A1
            FontSetting fontSetting = new FontSetting(0, cell.StringValue.Length, workbook.Worksheets);

            try
            {
                // Tillämpa WordArt-stil på teckensnittinställningen
                fontSetting.SetWordArtStyle(PresetWordArtStyle.WordArtStyle3);

                Console.WriteLine("WordArt style applied successfully to the text.");
                
                // Visa effekten genom att spara arbetsboken
                worksheet.AutoFitColumn(0);
                worksheet.AutoFitRow(0);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetWordArtStyle method: {ex.Message}");
            }
            
            // Spara resultatet
            workbook.Save("FontSettingMethodSetWordArtStyleDemo.xlsx");
        }
    }
}
```

### Se även

* enum [PresetWordArtStyle](../../../aspose.cells.drawing/presetwordartstyle/)
* class [FontSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


