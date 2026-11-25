---
title: "ImageOrPrintOptions.ImageType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ImageOrPrintOptions. Ottiene o imposta il formato delle immagini generate. valore predefinito PNG"
type: docs
url: /it/net/aspose.cells.rendering/imageorprintoptions/imagetype/
---
## ImageOrPrintOptions.ImageType property

Ottiene o imposta il formato delle immagini generate. valore predefinito: PNG.

```csharp
public virtual ImageType ImageType { get; set; }
```

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyImageTypeDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test SVG Image");

            // Imposta le opzioni di salvataggio HTML con il tipo di immagine SVG
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ImageOptions.ImageType = ImageType.Svg;
            options.ExportActiveWorksheetOnly = true;

            // Salva la cartella di lavoro come HTML
            string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "output.html");
            workbook.Save(outputPath, options);

            Console.WriteLine("File saved with SVG images: " + outputPath);
        }
    }
}
```

### Vedi anche

* enum [ImageType](../../../aspose.cells.drawing/imagetype/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


