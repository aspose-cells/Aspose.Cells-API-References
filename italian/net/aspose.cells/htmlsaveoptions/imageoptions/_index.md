---
title: "HtmlSaveOptions.ImageOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Ottieni l'oggetto ImageOrPrintOptions prima dell'esportazione"
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/imageoptions/
---
## HtmlSaveOptions.ImageOptions property

Ottieni l'oggetto ImageOrPrintOptions prima dell'esportazione

```csharp
public ImageOrPrintOptions ImageOptions { get; }
```

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyImageOptionsDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample HTML Export");
            
            // Imposta le opzioni di salvataggio HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportImagesAsBase64 = true;
            
            // Configura le opzioni immagine
            ImageOrPrintOptions imageOptions = saveOptions.ImageOptions;
            imageOptions.ImageType = ImageType.Svg;
            imageOptions.HorizontalResolution = 300;
            imageOptions.VerticalResolution = 300;
            
            // Salva la cartella di lavoro con le opzioni HTML
            string outputPath = "output.html";
            workbook.Save(outputPath, saveOptions);
            
            Console.WriteLine("HTML file saved with SVG images.");
        }
    }
}
```

### Vedi anche

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


