---
title: "HtmlSaveOptions.IsExpImageToTempDir"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlSaveOptions-Eigenschaft. Gibt an, ob Bilddateien in ein temporäres Verzeichnis exportiert werden. Nur beim Speichern in einen HTML-Stream"
type: docs
url: /de/net/aspose.cells/htmlsaveoptions/isexpimagetotempdir/
---
## HtmlSaveOptions.IsExpImageToTempDir property

Gibt an, ob Bilddateien in ein temporäres Verzeichnis exportiert werden. Nur beim Speichern in einen HTML‑Stream.

```csharp
public bool IsExpImageToTempDir { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyIsExpImageToTempDirDemo
    {
        public static void Run()
        {
            // Beispiel-Arbeitsmappe mit einem Bild erstellen
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispielbild zum Arbeitsblatt hinzufügen
            worksheet.Pictures.Add(0, 0, "https://www.aspose.com/templates/aspose/App_Themes/V3/images/cells/header/aspose_cells-for-net.png");

            // HTML-Speicheroptionen festlegen mit aktiviertem IsExpImageToTempDir
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.IsExpImageToTempDir = true;
            options.ExportImagesAsBase64 = false; // Ensure images are exported as separate files

            // Speichere die Arbeitsmappe als HTML
            workbook.Save("output.html", options);
            
            Console.WriteLine("HTML saved with images exported to temp directory.");
        }
    }
}
```

### Siehe auch

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


