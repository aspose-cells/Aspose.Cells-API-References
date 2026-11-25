---
title: "ImageOrPrintOptions.GridlineType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ImageOrPrintOptions. Ottiene o imposta il tipo di linea della griglia"
type: docs
url: /it/net/aspose.cells.rendering/imageorprintoptions/gridlinetype/
---
## ImageOrPrintOptions.GridlineType property

Ottiene o imposta il tipo di griglia.

```csharp
public GridlineType GridlineType { get; set; }
```

### Osservazioni

Il valore predefinito è il tipo Dotted.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyGridlineTypeDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e popola con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Book");
            worksheet.Cells["B2"].PutValue("$19.99");
            worksheet.Cells["A3"].PutValue("Pen");
            worksheet.Cells["B3"].PutValue("$2.99");

            // Crea un'istanza di ImageOrPrintOptions
            ImageOrPrintOptions imageOptions = new ImageOrPrintOptions
            {
                ImageType = ImageType.Png,
                GridlineType = GridlineType.Dotted // Use valid enum value
            };

            // Visualizza il tipo di linea della griglia corrente
            Console.WriteLine("Initial GridlineType: " + imageOptions.GridlineType);

            // Renderizza il foglio di lavoro con il tipo di linea della griglia iniziale
            SheetRender solidLineRenderer = new SheetRender(worksheet, imageOptions);
            solidLineRenderer.ToImage(0, "SolidGridlines.png");

            // Modifica il tipo di linea della griglia e renderizza nuovamente
            imageOptions.GridlineType = GridlineType.Hair; // Use valid enum value
            Console.WriteLine("\nModified GridlineType: " + imageOptions.GridlineType);

            SheetRender dashedLineRenderer = new SheetRender(worksheet, imageOptions);
            dashedLineRenderer.ToImage(0, "DashedGridlines.png");

            Console.WriteLine("Generated images demonstrate different gridline styles.");
        }
    }
}
```

### Vedi anche

* enum [GridlineType](../../../aspose.cells/gridlinetype/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


