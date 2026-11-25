---
title: "ImageOrPrintOptions.EmbededImageNameInSvg"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "ImageOrPrintOptions property. Indica il nome file dell'immagine incorporata in svg. Deve essere un percorso completo con directory, ad esempio cxpsEmbedded"
type: docs
url: /it/net/aspose.cells.rendering/imageorprintoptions/embededimagenameinsvg/
---
## ImageOrPrintOptions.EmbededImageNameInSvg property

Indica il nome file dell'immagine incorporata in SVG. Deve essere un percorso completo con directory, ad esempio "c:\\xpsEmbedded"

```csharp
[Obsolete("Images are now always embedded in Svg with base64 format, please remove this property.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string EmbededImageNameInSvg { get; set; }
```

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, rimuovi questa proprietà perché le immagini sono ora sempre incorporate in Svg con formato base64. Questa proprietà sarà rimossa tra 12 mesi a partire da aprile 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class ImageOrPrintOptionsPropertyEmbededImageNameInSvgDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e accedi al primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Genera un'immagine semplice in memoria e aggiungila al foglio di lavoro
            byte[] redPngBytes = Convert.FromBase64String("iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAYAAAAfFcSJAAAADUlEQVR42mNkYPhfDwAChwGA60e6kgAAAABJRU5ErkJggg==");
            worksheet.Pictures.Add(0, 0, new MemoryStream(redPngBytes));

            // Crea opzioni di rendering dell'immagine con formato SVG
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = ImageType.Svg
            };

            // Visualizza il percorso corrente dell'immagine incorporata
            Console.WriteLine("Initial EmbededImageNameInSvg: " + options.EmbededImageNameInSvg);

            // Configura una nuova directory per le immagini incorporate
            string imageDir = "svg_embedded_images/";
            options.EmbededImageNameInSvg = imageDir;
            Directory.CreateDirectory(imageDir);

            // Esegui il rendering del foglio di lavoro in SVG con le opzioni configurate
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "worksheet_output.svg");

            Console.WriteLine("Generated SVG with embedded images in: " + Path.GetFullPath(imageDir));
        }
    }
}
```

### Vedi anche

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


