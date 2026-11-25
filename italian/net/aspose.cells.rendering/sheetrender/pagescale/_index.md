---
title: "SheetRender.PageScale"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SheetRender. Ottiene la scala di pagina calcolata del foglio. Restituisce la scala impostata se Zoom è impostato. Altrimenti restituisce la scala calcolata secondo FitToPagesWide e FitToPagesTall"
type: docs
url: /it/net/aspose.cells.rendering/sheetrender/pagescale/
---
## SheetRender.PageScale property

Ottiene la scala di pagina calcolata del foglio. Restituisce la scala impostata se [`Zoom`](../../../aspose.cells/pagesetup/zoom/) è impostato. Altrimenti, restituisce la scala calcolata secondo [`FitToPagesWide`](../../../aspose.cells/pagesetup/fittopageswide/) e [`FitToPagesTall`](../../../aspose.cells/pagesetup/fittopagestall/).

```csharp
public double PageScale { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetRenderPropertyPageScaleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook con dati di esempio
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Aggiungi dati di esempio alle celle
            for (int i = 0; i < 10; i++)
            {
                sheet.Cells[i, 0].PutValue($"Item {i + 1}");
                sheet.Cells[i, 1].PutValue((i + 1) * 10);
            }

            // Crea opzioni di immagine o stampa
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            
            // Crea il rendering del foglio
            SheetRender sheetRender = new SheetRender(sheet, options);
            
            // Ottieni e visualizza la scala di pagina calcolata
            double pageScale = sheetRender.PageScale;
            Console.WriteLine($"Calculated Page Scale: {pageScale}");
        }
    }
}
```

### Vedi anche

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


