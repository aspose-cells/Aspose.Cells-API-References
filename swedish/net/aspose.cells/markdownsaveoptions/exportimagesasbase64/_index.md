---
title: "MarkdownSaveOptions.ExportImagesAsBase64"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MarkdownSaveOptions‑egenskap. Anger om bilder sparas i Base64‑format till Markdown. Standardvärdet är true"
type: docs
url: /sv/net/aspose.cells/markdownsaveoptions/exportimagesasbase64/
---
## MarkdownSaveOptions.ExportImagesAsBase64 property

Anger om bilder sparas i Base64-format till Markdown. Standardvärdet är sant.

```csharp
public bool ExportImagesAsBase64 { get; set; }
```

### Anmärkningar

När denna egenskap är satt till true exporteras bilddata direkt i img‑elementen och separata filer skapas inte.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownSaveOptionsPropertyExportImagesAsBase64Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata och en bild
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B1"].PutValue("With Image");

            // Lägg till en bild i kalkylbladet
            int imageIndex = worksheet.Pictures.Add(1, 1, "sample.png");

            try
            {
                // Skapa en instans av MarkdownSaveOptions
                MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

                // Visa standardvärdet för ExportImagesAsBase64
                Console.WriteLine("Default ExportImagesAsBase64 value: " + saveOptions.ExportImagesAsBase64);

                // Ange ExportImagesAsBase64 till false för att demonstrera egenskapen
                saveOptions.ExportImagesAsBase64 = false;
                Console.WriteLine("ExportImagesAsBase64 set to: " + saveOptions.ExportImagesAsBase64);

                // Spara med ExportImagesAsBase64 = false
                workbook.Save("MarkdownImagesAsFiles.md", saveOptions);

                // Ange ExportImagesAsBase64 till true
                saveOptions.ExportImagesAsBase64 = true;
                Console.WriteLine("ExportImagesAsBase64 set to: " + saveOptions.ExportImagesAsBase64);

                // Spara med ExportImagesAsBase64 = true
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

### Se även

* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


