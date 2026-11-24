---
title: "ImageOrPrintOptions.PageCount"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ImageOrPrintOptions-Eigenschaft. Gibt die zu speichernde Seitenanzahl zurück oder legt sie fest."
type: docs
url: /de/net/aspose.cells.rendering/imageorprintoptions/pagecount/
---
## ImageOrPrintOptions.PageCount property

Liest oder legt die Anzahl der zu speichernden Seiten fest.

```csharp
public int PageCount { get; set; }
```

### Hinweise

Standard ist System.Int32.MaxValue, was bedeutet, dass alle Seiten gerendert werden.

### Beispiele

```csharp
using System;
using System.IO;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyPageCountDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten zum Arbeitsblatt hinzufügen
            worksheet.Cells["A1"].PutValue("Page 1 Data");
            worksheet.Cells["A2"].PutValue("Sample Content");
            worksheet.Cells["A3"].PutValue("Demo for PageCount");
            
            // Lege den Druckbereich und die Seiteneinrichtung fest
            worksheet.PageSetup.PrintArea = "A1:A3";
            worksheet.PageSetup.LeftMargin = 0;
            worksheet.PageSetup.RightMargin = 0;
            worksheet.PageSetup.TopMargin = 0;
            worksheet.PageSetup.BottomMargin = 0;

            // Bild- oder Druckoptionen erstellen
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png; // Fully qualified namespace AsposeCellsExamples = 1; // Demonstrating PageCount property
            options.OnlyArea = true;

            // Render das Arbeitsblatt zu einem Bild
            SheetRender renderer = new SheetRender(worksheet, options);
            using (MemoryStream stream = new MemoryStream())
            {
                renderer.ToImage(0, stream);
                
                // Speichere das Bild in einer Datei
                string outputPath = "output.png";
                File.WriteAllBytes(outputPath, stream.ToArray());
                Console.WriteLine($"Output saved to: {outputPath}");
            }
        }
    }
}
```

### Siehe auch

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


