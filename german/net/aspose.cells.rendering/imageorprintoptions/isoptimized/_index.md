---
title: "ImageOrPrintOptions.IsOptimized"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ImageOrPrintOptions-Eigenschaft. Gibt an, ob die Ausgabeelemente optimiert werden sollen."
type: docs
url: /de/net/aspose.cells.rendering/imageorprintoptions/isoptimized/
---
## ImageOrPrintOptions.IsOptimized property

Gibt an, ob die Ausgabeelemente optimiert werden sollen.

```csharp
public bool IsOptimized { get; set; }
```

### Hinweise

Standardwert ist false. Derzeit, wenn diese Eigenschaft auf true gesetzt wird, werden die folgenden Optimierungen durchgeführt: 1. Optimierung der Rahmenlinien. 2. Optimierung der Dateigröße beim Rendern zu einem Svg-Bild.

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyIsOptimizedDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten zu Zellen hinzu
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    sheet.Cells[i, j].PutValue($"Data {i}-{j}");
                }
            }

            // Bildrender-Optionen einrichten
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            options.OnePagePerSheet = true;
            
            // Demonstriere die IsOptimized-Eigenschaft
            options.IsOptimized = true; // Enable optimization
            
            // Render das Blatt zu einem Bild
            SheetRender renderer = new SheetRender(sheet, options);
            MemoryStream stream = new MemoryStream();
            renderer.ToImage(0, stream);
            
            Console.WriteLine($"Image rendered with optimization: {options.IsOptimized}");
            Console.WriteLine($"Image size: {stream.Length} bytes");
        }
    }
}
```

### Siehe auch

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


