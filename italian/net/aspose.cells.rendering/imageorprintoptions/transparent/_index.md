---
title: "ImageOrPrintOptions.Transparent"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ImageOrPrintOptions. Indica se lo sfondo dell'immagine generata deve essere trasparente"
type: docs
url: /it/net/aspose.cells.rendering/imageorprintoptions/transparent/
---
## ImageOrPrintOptions.Transparent property

Indica se lo sfondo dell'immagine generata deve essere trasparente.

```csharp
public bool Transparent { get; set; }
```

### Osservazioni

Il valore predefinito è false. Questo significa che lo sfondo delle immagini generate è bianco.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyTransparentDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Transparent Image Demo");
            
            // Imposta le opzioni di salvataggio HTML con immagine PNG trasparente
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ImageOptions.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            options.ImageOptions.Transparent = true;
            options.ExportImagesAsBase64 = true;

            // Salva la cartella di lavoro con opzioni immagine trasparente
            workbook.Save("output.html", options);
            
            Console.WriteLine("HTML with transparent images saved successfully.");
        }
    }
}
```

### Vedi anche

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


