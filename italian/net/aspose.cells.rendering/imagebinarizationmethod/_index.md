---
title: "Enum ImageBinarizationMethod"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Rendering.ImageBinarizationMethod enum. Specifica il metodo usato per binarizzare l'immagine"
type: docs
url: /it/net/aspose.cells.rendering/imagebinarizationmethod/
---
## ImageBinarizationMethod enumeration

Specifica il metodo utilizzato per binarizzare l'immagine.

```csharp
public enum ImageBinarizationMethod
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Threshold | `0` | Specifica il metodo di soglia. |
| FloydSteinbergDithering | `1` | Specifica la dithering usando il metodo di diffusione dell'errore di Floyd‑Steinberg. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class RenderingClassImageBinarizationMethodDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro con dati di prova
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Popola le celle con valori a gradiente per la dimostrazione
            for (int row = 0; row < 50; row++)
            {
                for (int col = 0; col < 10; col++)
                {
                    worksheet.Cells[row, col].PutValue((double)(row * col) / 500);
                }
            }

            // Configura le opzioni di rendering dell'immagine
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = ImageType.Tiff,
                TiffCompression = TiffCompression.CompressionCCITT4,
                TiffBinarizationMethod = ImageBinarizationMethod.FloydSteinbergDithering
            };

            // Crea il rendering del foglio con le opzioni configurate
            SheetRender renderer = new SheetRender(worksheet, options);
            
            // Renderizza la prima pagina del foglio di lavoro in immagine con binarizzazione
            renderer.ToImage(0, "BinarizedOutput.tiff");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


