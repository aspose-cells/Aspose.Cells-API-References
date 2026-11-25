---
title: "PdfSaveOptions.ImageType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PdfSaveOptions. Rappresenta il tipo di immagine durante la conversione del grafico e della forma"
type: docs
url: /it/net/aspose.cells/pdfsaveoptions/imagetype/
---
## PdfSaveOptions.ImageType property

Rappresenta il tipo di immagine durante la conversione del grafico e della forma.

```csharp
[Obsolete("Chart and Shape are always rendered as vector elements(e.g. point, line) for rendering quality.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ImageFormat ImageType { get; set; }
```

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, Chart e Shape vengono sempre renderizzati come elementi vettoriali (ad es. punto, linea) per la qualità del rendering. Questa proprietà sarà rimossa 12 mesi dopo, a partire da giugno 2022. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;
    using System.Drawing.Imaging;

    public class PdfSaveOptionsPropertyImageTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Crea un foglio di lavoro di esempio con alcuni dati
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data for PDF Export";
            worksheet.Cells["A2"].Value = "Demonstrating ImageType Property";

            try
            {
                // Crea le opzioni di salvataggio PDF
                PdfSaveOptions saveOptions = new PdfSaveOptions();

                // Visualizza il valore predefinito di ImageType
                Console.WriteLine("Default ImageType: " + saveOptions.ImageType);

                // Imposta un valore diverso per ImageType
                saveOptions.ImageType = ImageFormat.Png;
                Console.WriteLine("Updated ImageType: " + saveOptions.ImageType);

                // Salva la cartella di lavoro come PDF con l'ImageType specificato
                workbook.Save("ImageTypeDemo.pdf", saveOptions);

                Console.WriteLine("PDF saved with ImageType setting applied.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


