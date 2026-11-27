---
title: "FontSettingCollection.SetWordArtStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FontSettingCollection-metod. Ställer in den förinställda WordArt-stilen"
type: docs
url: /sv/net/aspose.cells.drawing.texts/fontsettingcollection/setwordartstyle/
---
## FontSettingCollection.SetWordArtStyle method

Ställer in den förinställda WordArt-stilen.

```csharp
public void SetWordArtStyle(PresetWordArtStyle style)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| style | PresetWordArtStyle | Den förinställda WordArt-stilen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingCollectionMethodSetWordArtStyleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en textruta i kalkylbladet
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            var fontSettingCollection = textBox.TextBody;

            // Ange ursprunglig text
            fontSettingCollection.Text = "Sample Text for WordArt Styling";

            try
            {
                // Anropa SetWordArtStyle-metoden med WordArtStyle7 (Gradientfyllning – Blå, Accent 1, Reflektion)
                fontSettingCollection.SetWordArtStyle(PresetWordArtStyle.WordArtStyle7);

                Console.WriteLine("WordArt style applied successfully to the text box.");

                // Spara arbetsboken för att visa effekten
                workbook.Save("FontSettingCollectionSetWordArtStyleDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetWordArtStyle method: {ex.Message}");
            }
        }
    }
}
```

### Se även

* enum [PresetWordArtStyle](../../../aspose.cells.drawing/presetwordartstyle/)
* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


