---
title: "HtmlSaveOptions.ExportImagesAsBase64"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlSaveOptions-Eigenschaft. Gibt an, ob Bilder im Base64-Format in HTML, MHTML oder EPUB gespeichert werden"
type: docs
url: /de/net/aspose.cells/htmlsaveoptions/exportimagesasbase64/
---
## HtmlSaveOptions.ExportImagesAsBase64 property

Gibt an, ob Bilder im Base64-Format in html, MHTML oder EPUB gespeichert werden.

```csharp
public bool ExportImagesAsBase64 { get; set; }
```

### Hinweise

Wenn diese Eigenschaft auf true gesetzt ist, werden Bilddaten direkt in den img-Elementen exportiert und separate Dateien werden nicht erstellt.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportImagesAsBase64Demo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge ein Bild zum Arbeitsblatt hinzu
            worksheet.Pictures.Add(0, 0, "example.jpg");
            
            // HTML‑Speicheroptionen erstellen
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Setzen Sie ExportImagesAsBase64 auf true, um Bilder als Base64-Zeichenketten einzubetten
            saveOptions.ExportImagesAsBase64 = true;
            
            // Speichern Sie die Arbeitsmappe als HTML mit eingebetteten Bildern
            workbook.Save("output.html", saveOptions);
            
            Console.WriteLine("HTML with embedded images saved successfully.");
        }
    }
}
```

### Siehe auch

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


