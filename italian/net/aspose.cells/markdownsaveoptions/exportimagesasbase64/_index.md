---
title: "MarkdownSaveOptions.ExportImagesAsBase64"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà MarkdownSaveOptions. Specifica se le immagini vengono salvate in formato Base64 nel Markdown. Il valore predefinito è true"
type: docs
url: /it/net/aspose.cells/markdownsaveoptions/exportimagesasbase64/
---
## MarkdownSaveOptions.ExportImagesAsBase64 property

Specifica se le immagini sono salvate in formato Base64 nel Markdown. Il valore predefinito è true.

```csharp
public bool ExportImagesAsBase64 { get; set; }
```

### Osservazioni

Quando questa proprietà è impostata su true, i dati dell'immagine vengono esportati direttamente negli elementi img e non vengono creati file separati.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownSaveOptionsPropertyExportImagesAsBase64Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio e un'immagine
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B1"].PutValue("With Image");

            // Aggiungi un'immagine al foglio di lavoro
            int imageIndex = worksheet.Pictures.Add(1, 1, "sample.png");

            try
            {
                // Crea un'istanza di MarkdownSaveOptions
                MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

                // Visualizza il valore predefinito di ExportImagesAsBase64
                Console.WriteLine("Default ExportImagesAsBase64 value: " + saveOptions.ExportImagesAsBase64);

                // Imposta ExportImagesAsBase64 su false per dimostrare la proprietà
                saveOptions.ExportImagesAsBase64 = false;
                Console.WriteLine("ExportImagesAsBase64 set to: " + saveOptions.ExportImagesAsBase64);

                // Salva con ExportImagesAsBase64 = false
                workbook.Save("MarkdownImagesAsFiles.md", saveOptions);

                // Imposta ExportImagesAsBase64 su true
                saveOptions.ExportImagesAsBase64 = true;
                Console.WriteLine("ExportImagesAsBase64 set to: " + saveOptions.ExportImagesAsBase64);

                // Salva con ExportImagesAsBase64 = true
                workbook.Save("MarkdownImagesAsBase64.md", saveOptions);

                Console.WriteLine("Markdown files saved with different ExportImagesAsBase64 settings.");
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

* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


