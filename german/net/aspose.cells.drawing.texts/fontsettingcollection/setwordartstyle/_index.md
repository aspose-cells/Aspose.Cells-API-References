---
title: "FontSettingCollection.SetWordArtStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FontSettingCollection‑Methode. Legt den vordefinierten WordArt‑Stil fest"
type: docs
url: /de/net/aspose.cells.drawing.texts/fontsettingcollection/setwordartstyle/
---
## FontSettingCollection.SetWordArtStyle method

Setzt den voreingestellten WordArt-Stil.

```csharp
public void SetWordArtStyle(PresetWordArtStyle style)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Stil | PresetWordArtStyle | Der voreingestellte WordArt-Stil. |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein Textfeld zum Arbeitsblatt hinzu
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            var fontSettingCollection = textBox.TextBody;

            // Initialen Text festlegen
            fontSettingCollection.Text = "Sample Text for WordArt Styling";

            try
            {
                // Rufe die SetWordArtStyle‑Methode mit WordArtStyle7 (Verlaufsfüllung – Blau, Akzent 1, Spiegelung) auf
                fontSettingCollection.SetWordArtStyle(PresetWordArtStyle.WordArtStyle7);

                Console.WriteLine("WordArt style applied successfully to the text box.");

                // Arbeitsmappe speichern, um den Effekt zu zeigen
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

### Siehe auch

* enum [PresetWordArtStyle](../../../aspose.cells.drawing/presetwordartstyle/)
* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


