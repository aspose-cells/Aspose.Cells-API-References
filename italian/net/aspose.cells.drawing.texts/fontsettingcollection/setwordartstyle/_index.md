---
title: "FontSettingCollection.SetWordArtStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo FontSettingCollection. Imposta lo stile WordArt predefinito"
type: docs
url: /it/net/aspose.cells.drawing.texts/fontsettingcollection/setwordartstyle/
---
## FontSettingCollection.SetWordArtStyle method

Imposta lo stile predefinito di WordArt.

```csharp
public void SetWordArtStyle(PresetWordArtStyle style)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stile | PresetWordArtStyle | Lo stile WordArt predefinito. |

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una casella di testo al foglio di lavoro
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            var fontSettingCollection = textBox.TextBody;

            // Imposta il testo iniziale
            fontSettingCollection.Text = "Sample Text for WordArt Styling";

            try
            {
                // Chiama il metodo SetWordArtStyle con WordArtStyle7 (Riempimento gradiente - Blu, Accento 1, Riflesso)
                fontSettingCollection.SetWordArtStyle(PresetWordArtStyle.WordArtStyle7);

                Console.WriteLine("WordArt style applied successfully to the text box.");

                // Salva la cartella di lavoro per mostrare l'effetto
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

### Vedi anche

* enum [PresetWordArtStyle](../../../aspose.cells.drawing/presetwordartstyle/)
* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


