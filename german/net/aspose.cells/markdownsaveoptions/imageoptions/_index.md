---
title: "MarkdownSaveOptions.ImageOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MarkdownSaveOptions-Eigenschaft. Ruft das ImageOrPrintOptions‑Objekt vor dem Exportieren ab"
type: docs
url: /de/net/aspose.cells/markdownsaveoptions/imageoptions/
---
## MarkdownSaveOptions.ImageOptions property

Rufen Sie das ImageOrPrintOptions‑Objekt vor dem Exportieren ab.

```csharp
public ImageOrPrintOptions ImageOptions { get; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Erstelle ein Beispiel-Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge einige Daten hinzu, um das Beispiel sinnvoll zu machen.
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["A2"].Value = "Image Options Demo";

            try
            {
                // Erstelle eine MarkdownSaveOptions-Instanz.
                MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

                // Greifen Sie auf die ImageOptions-Eigenschaft zu (nur lesbar)
                ImageOrPrintOptions imageOptions = saveOptions.ImageOptions;

                // Zeigen Sie die aktuellen Werte der ImageOptions-Eigenschaften an
                Console.WriteLine("ImageOptions properties:");
                Console.WriteLine($"HorizontalResolution: {imageOptions.HorizontalResolution}");
                Console.WriteLine($"VerticalResolution: {imageOptions.VerticalResolution}");
                Console.WriteLine($"ImageType: {imageOptions.ImageType}");
                Console.WriteLine($"Quality: {imageOptions.Quality}");
                Console.WriteLine($"Transparent: {imageOptions.Transparent}");

                // Speichern Sie die Arbeitsmappe mit den aktuellen Optionen
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

### Siehe auch

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


