---
title: "ImageOrPrintOptions.OnlyArea"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ImageOrPrintOptions. Se questa proprietà è true, verrà prodotto un unico Area e nessuna scala avrà effetto"
type: docs
url: /it/net/aspose.cells.rendering/imageorprintoptions/onlyarea/
---
## ImageOrPrintOptions.OnlyArea property

Se questa proprietà è true, verrà output una sola Area e nessuna scala avrà effetto.

```csharp
public bool OnlyArea { get; set; }
```

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyOnlyAreaDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio alle celle
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Imposta le opzioni immagine con la proprietà OnlyArea
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            options.OnlyArea = true; // Only render the used area

            // Renderizza il foglio di lavoro in immagine
            SheetRender sr = new SheetRender(worksheet, options);
            using (MemoryStream ms = new MemoryStream())
            {
                sr.ToImage(0, ms);
                Console.WriteLine("Worksheet rendered to image with OnlyArea=true");
            }
        }
    }
}
```

### Vedi anche

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


