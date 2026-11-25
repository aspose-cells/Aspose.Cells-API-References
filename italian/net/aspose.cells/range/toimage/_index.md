---
title: "Range.ToImage"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Range. Converte l'intervallo in immagine"
type: docs
url: /it/net/aspose.cells/range/toimage/
---
## Range.ToImage method

Converte l'intervallo in immagine.

```csharp
public byte[] ToImage(ImageOrPrintOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| opzioni | ImageOrPrintOptions | Le opzioni per convertire questo intervallo in immagine |

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RangeMethodToImageWithImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro dal file Excel di esempio
            Workbook workbook = new Workbook("example.xlsx");
            
            // Ottieni il primo foglio di lavoro e le sue celle
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Crea l'intervallo A1:J25
            Aspose.Cells.Range range = cells.CreateRange("A1:J25");
            
            // Crea opzioni immagine
            ImageOrPrintOptions options = new ImageOrPrintOptions()
            {
                ImageType = Aspose.Cells.Drawing.ImageType.Png,
                HorizontalResolution = 300,
                VerticalResolution = 300
            };
            
            // Converti l'intervallo in immagine
            byte[] imageData = range.ToImage(options);
            
            // Salva l'immagine su file
            File.WriteAllBytes("range_output.png", imageData);
        }
    }
}
```

### Vedi anche

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


