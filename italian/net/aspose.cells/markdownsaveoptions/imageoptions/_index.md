---
title: "MarkdownSaveOptions.ImageOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà MarkdownSaveOptions. Ottieni l'oggetto ImageOrPrintOptions prima dell'esportazione"
type: docs
url: /it/net/aspose.cells/markdownsaveoptions/imageoptions/
---
## MarkdownSaveOptions.ImageOptions property

Ottieni l'oggetto ImageOrPrintOptions prima dell'esportazione

```csharp
public ImageOrPrintOptions ImageOptions { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class MarkdownSaveOptionsPropertyImageOptionsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Crea un foglio di lavoro di esempio
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati per rendere l'esempio significativo
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["A2"].Value = "Image Options Demo";

            try
            {
                // Crea un'istanza di MarkdownSaveOptions
                MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

                // Accedi alla proprietà ImageOptions (sola lettura)
                ImageOrPrintOptions imageOptions = saveOptions.ImageOptions;

                // Visualizza i valori attuali delle proprietà ImageOptions
                Console.WriteLine("ImageOptions properties:");
                Console.WriteLine($"HorizontalResolution: {imageOptions.HorizontalResolution}");
                Console.WriteLine($"VerticalResolution: {imageOptions.VerticalResolution}");
                Console.WriteLine($"ImageType: {imageOptions.ImageType}");
                Console.WriteLine($"Quality: {imageOptions.Quality}");
                Console.WriteLine($"Transparent: {imageOptions.Transparent}");

                // Salva la cartella di lavoro con le opzioni correnti
                workbook.Save("ImageOptionsDemo.md", saveOptions);

                Console.WriteLine("Markdown file saved successfully with ImageOptions demonstrated.");
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

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


