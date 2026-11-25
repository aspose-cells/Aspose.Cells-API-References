---
title: "SheetRender.SheetRender"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore di SheetRender. La costruzione di SheetRender richiede worksheet e ImageOrPrintOptions come parametri"
type: docs
url: /it/net/aspose.cells.rendering/sheetrender/sheetrender/
---
## SheetRender constructor

la costruzione di SheetRender, richiede foglio di lavoro e ImageOrPrintOptions come parametri

```csharp
public SheetRender(Worksheet worksheet, ImageOrPrintOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| worksheet | Worksheet | Indicare quale foglio di calcolo deve essere renderizzato. |
| opzioni | ImageOrPrintOptions | ImageOrPrintOptions contiene alcune proprietà dell'immagine di output |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetRenderMethodCtorWithWorksheetImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // Creare una cartella di lavoro e aggiungere alcuni dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio alle celle
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Crea opzioni di immagine/stampa
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            options.OnePagePerSheet = true;

            // Creare SheetRender con Worksheet e ImageOrPrintOptions
            SheetRender render = new SheetRender(worksheet, options);

            // Conteggio delle pagine di output
            Console.WriteLine("Page count: " + render.PageCount);

            // Salvare l'immagine renderizzata
            render.ToImage(0, "output.png");
        }
    }
}
```

### Vedi anche

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [ImageOrPrintOptions](../../imageorprintoptions/)
* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


