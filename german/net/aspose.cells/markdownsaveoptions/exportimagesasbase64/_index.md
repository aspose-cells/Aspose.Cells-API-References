---
title: "MarkdownSaveOptions.ExportImagesAsBase64"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MarkdownSaveOptions-Eigenschaft. Gibt an, ob Bilder im Base64‑Format in Markdown gespeichert werden. Der Standardwert ist true"
type: docs
url: /de/net/aspose.cells/markdownsaveoptions/exportimagesasbase64/
---
## MarkdownSaveOptions.ExportImagesAsBase64 property

Gibt an, ob Bilder im Base64-Format in Markdown gespeichert werden. Der Standardwert ist true.

```csharp
public bool ExportImagesAsBase64 { get; set; }
```

### Hinweise

Wenn diese Eigenschaft auf true gesetzt ist, werden Bilddaten direkt in den img-Elementen exportiert und separate Dateien werden nicht erstellt.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownSaveOptionsPropertyExportImagesAsBase64Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten und ein Bild hinzufügen
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B1"].PutValue("With Image");

            // Füge ein Bild zum Arbeitsblatt hinzu
            int imageIndex = worksheet.Pictures.Add(1, 1, "sample.png");

            try
            {
                // Erstelle eine MarkdownSaveOptions-Instanz.
                MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

                // Standardwert von ExportImagesAsBase64 anzeigen
                Console.WriteLine("Default ExportImagesAsBase64 value: " + saveOptions.ExportImagesAsBase64);

                // ExportImagesAsBase64 auf false setzen, um die Eigenschaft zu demonstrieren
                saveOptions.ExportImagesAsBase64 = false;
                Console.WriteLine("ExportImagesAsBase64 set to: " + saveOptions.ExportImagesAsBase64);

                // Speichern mit ExportImagesAsBase64 = false
                workbook.Save("MarkdownImagesAsFiles.md", saveOptions);

                // ExportImagesAsBase64 auf true setzen
                saveOptions.ExportImagesAsBase64 = true;
                Console.WriteLine("ExportImagesAsBase64 set to: " + saveOptions.ExportImagesAsBase64);

                // Speichern mit ExportImagesAsBase64 = true
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

### Siehe auch

* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


