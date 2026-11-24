---
title: "ImageOrPrintOptions.OutputBlankPageWhenNothingToPrint"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ImageOrPrintOptions-Eigenschaft. Gibt an, ob eine leere Seite ausgegeben werden soll, wenn nichts zu drucken ist"
type: docs
url: /de/net/aspose.cells.rendering/imageorprintoptions/outputblankpagewhennothingtoprint/
---
## ImageOrPrintOptions.OutputBlankPageWhenNothingToPrint property

Gibt an, ob eine leere Seite ausgegeben werden soll, wenn nichts zu drucken ist.

```csharp
public bool OutputBlankPageWhenNothingToPrint { get; set; }
```

### Hinweise

Standard ist false.

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyOutputBlankPageWhenNothingToPrintDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine neue leere Arbeitsmappe
            Workbook workbook = new Workbook();
            
            // Greifen Sie auf das erste Arbeitsblatt zu, das leer ist
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bild- oder Druckoptionen festlegen
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            options.OnePagePerSheet = true;
            
            // Demonstrieren Sie die OutputBlankPageWhenNothingToPrint-Eigenschaft
            options.OutputBlankPageWhenNothingToPrint = true;
            
            // Rendern Sie das Blatt
            SheetRender renderer = new SheetRender(worksheet, options);
            
            // Die Ausgabe erzeugt weiterhin eine leere Seite aufgrund der Eigenschaftseinstellung
            Console.WriteLine("Page count with OutputBlankPageWhenNothingToPrint=true: " + renderer.PageCount);
            
            // Speichern Sie die erste Seite im Memory-Stream
            MemoryStream stream = new MemoryStream();
            renderer.ToImage(0, stream);
            Console.WriteLine("Image data length: " + stream.ToArray().Length);
            
            // Setzen Sie jetzt die Eigenschaft auf false
            options.OutputBlankPageWhenNothingToPrint = false;
            SheetRender renderer2 = new SheetRender(worksheet, options);
            
            // Die Ausgabe hat jetzt null Seiten
            Console.WriteLine("Page count with OutputBlankPageWhenNothingToPrint=false: " + renderer2.PageCount);
        }
    }
}
```

### Siehe auch

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


