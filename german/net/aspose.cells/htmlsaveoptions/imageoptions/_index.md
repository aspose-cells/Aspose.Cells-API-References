---
title: "HtmlSaveOptions.ImageOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlSaveOptions-Eigenschaft. Holen Sie das ImageOrPrintOptions-Objekt vor dem Export"
type: docs
url: /de/net/aspose.cells/htmlsaveoptions/imageoptions/
---
## HtmlSaveOptions.ImageOptions property

Rufen Sie das ImageOrPrintOptions‑Objekt vor dem Exportieren ab.

```csharp
public ImageOrPrintOptions ImageOptions { get; }
```

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyImageOptionsDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample HTML Export");
            
            // HTML-Speicheroptionen festlegen
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportImagesAsBase64 = true;
            
            // Bildoptionen konfigurieren
            ImageOrPrintOptions imageOptions = saveOptions.ImageOptions;
            imageOptions.ImageType = ImageType.Svg;
            imageOptions.HorizontalResolution = 300;
            imageOptions.VerticalResolution = 300;
            
            // Speichere die Arbeitsmappe mit HTML-Optionen
            string outputPath = "output.html";
            workbook.Save(outputPath, saveOptions);
            
            Console.WriteLine("HTML file saved with SVG images.");
        }
    }
}
```

### Siehe auch

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


