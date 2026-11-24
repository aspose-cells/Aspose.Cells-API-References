---
title: "HtmlSaveOptions.ImageScalable"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlSaveOptions Eigenschaft. Gibt an, ob eine skalierbare Einheit zur Beschreibung der Bildbreite verwendet wird, wenn eine skalierbare Einheit zur Beschreibung der Spaltenbreite verwendet wird. Der Standardwert ist true."
type: docs
url: /de/net/aspose.cells/htmlsaveoptions/imagescalable/
---
## HtmlSaveOptions.ImageScalable property

Gibt an, ob eine skalierbare Einheit zur Beschreibung der Bildbreite verwendet wird, wenn eine skalierbare Einheit zur Beschreibung der Spaltenbreite verwendet wird. Der Standardwert ist true.

```csharp
public bool ImageScalable { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyImageScalableDemo
    {
        public static void Run()
        {
            // Beispiel-Arbeitsmappe mit einem Bild erstellen
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispielbild zum Arbeitsblatt hinzufügen
            int imgIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
            Aspose.Cells.Drawing.Picture picture = worksheet.Pictures[imgIndex];

            // HTML-Speicheroptionen mit ImageScalable-Eigenschaft festlegen
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ImageScalable = false; // Images won't scale with the HTML content
            
            // Speichere die Arbeitsmappe als HTML
            workbook.Save("output.html", saveOptions);
            
            Console.WriteLine("HTML file saved with ImageScalable set to false.");
        }
    }
}
```

### Siehe auch

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


