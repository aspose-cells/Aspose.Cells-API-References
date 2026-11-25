---
title: "ImageOrPrintOptions.SVGFitToViewPort"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ImageOrPrintOptions. se questa proprietà è true, l'SVG generato si adatterà alla viewport"
type: docs
url: /it/net/aspose.cells.rendering/imageorprintoptions/svgfittoviewport/
---
## ImageOrPrintOptions.SVGFitToViewPort property

Se questa proprietà è true, l'SVG generato si adatterà alla viewport.

```csharp
[Obsolete("Use SvgImageOptions.FitToViewPort property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool SVGFitToViewPort { get; set; }
```

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare [`FitToViewPort`](../../svgimageoptions/fittoviewport/). Questa proprietà sarà rimossa 12 mesi dopo, a partire da aprile 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertySVGFitToViewPortDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio alle celle
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(15);
            
            // Creare opzioni immagine per l'output SVG
            ImageOrPrintOptions opts = new ImageOrPrintOptions();
            opts.ImageType = Aspose.Cells.Drawing.ImageType.Svg;
            opts.OnePagePerSheet = true;
            opts.SVGFitToViewPort = true; // This is the key property being demonstrated
            
            // Renderizzare il foglio di lavoro in immagine SVG
            SheetRender sr = new SheetRender(worksheet, opts);
            sr.ToImage(0, "output.svg");
            
            Console.WriteLine("SVG file with SVGFitToViewPort=true created successfully.");
        }
    }
}
```

### Vedi anche

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


