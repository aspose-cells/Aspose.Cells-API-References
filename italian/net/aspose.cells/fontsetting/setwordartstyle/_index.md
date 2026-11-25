---
title: "FontSetting.SetWordArtStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo FontSetting. Imposta lo stile WordArt predefinito"
type: docs
url: /it/net/aspose.cells/fontsetting/setwordartstyle/
---
## FontSetting.SetWordArtStyle method

Imposta lo stile predefinito di WordArt.

```csharp
public void SetWordArtStyle(PresetWordArtStyle style)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stile | PresetWordArtStyle | Lo stile WordArt predefinito. |

### Osservazioni

Solo per il testo di forma/grafico.

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi del testo alla cella A1
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text for WordArt");

            // Crea impostazione del carattere per il testo nella cella A1
            FontSetting fontSetting = new FontSetting(0, cell.StringValue.Length, workbook.Worksheets);

            try
            {
                // Applica lo stile WordArt all'impostazione del carattere
                fontSetting.SetWordArtStyle(PresetWordArtStyle.WordArtStyle3);

                Console.WriteLine("WordArt style applied successfully to the text.");
                
                // Mostra l'effetto salvando la cartella di lavoro
                worksheet.AutoFitColumn(0);
                worksheet.AutoFitRow(0);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetWordArtStyle method: {ex.Message}");
            }
            
            // Salva il risultato
            workbook.Save("FontSettingMethodSetWordArtStyleDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [PresetWordArtStyle](../../../aspose.cells.drawing/presetwordartstyle/)
* class [FontSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


