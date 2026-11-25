---
title: "Classe WorkbookRender"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Rendering.WorkbookRender. Rappresenta il rendering di una cartella di lavoro. Il costruttore di questa classe deve essere usato dopo la modifica dello stile della cella di impostazione pagina"
type: docs
url: /it/net/aspose.cells.rendering/workbookrender/
---
## WorkbookRender class

Rappresenta il rendering di una cartella di lavoro. Il costruttore di questa classe deve essere utilizzato dopo la modifica di pagesetup e dello stile delle celle.

```csharp
public class WorkbookRender
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [WorkbookRender](workbookrender/)(Workbook, ImageOrPrintOptions) | La costruzione di WorkbookRender |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [PageCount](../../aspose.cells.rendering/workbookrender/pagecount/) { get; } | Ottiene il conteggio totale delle pagine della cartella di lavoro. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [CustomPrint](../../aspose.cells.rendering/workbookrender/customprint/)(bool, PrintPageEventArgs) | Il client può controllare le impostazioni della pagina della stampante quando stampa ogni pagina usando questa funzione. |
| [Dispose](../../aspose.cells.rendering/workbookrender/dispose/)() | Rilascia le risorse create e usate per il rendering. |
| [GetPageSizeInch](../../aspose.cells.rendering/workbookrender/getpagesizeinch/)(int) | Ottieni la dimensione della pagina in pollici dell'immagine di output. |
| [ToImage](../../aspose.cells.rendering/workbookrender/toimage/#toimage)(int) | Esegui il rendering di una pagina specifica in un oggetto Bitmap. |
| [ToImage](../../aspose.cells.rendering/workbookrender/toimage/#toimage_3)(Stream) | Esegui il rendering dell'intera cartella di lavoro come immagine Tiff in uno stream. |
| [ToImage](../../aspose.cells.rendering/workbookrender/toimage/#toimage_4)(string) | Esegui il rendering dell'intera cartella di lavoro come immagine Tiff in un file. |
| [ToImage](../../aspose.cells.rendering/workbookrender/toimage/#toimage_1)(int, Stream) | Esegui il rendering di una pagina specifica in uno stream. |
| [ToImage](../../aspose.cells.rendering/workbookrender/toimage/#toimage_2)(int, string) | Esegui il rendering di una pagina specifica in un file. |
| [ToPrinter](../../aspose.cells.rendering/workbookrender/toprinter/#toprinter)(PrinterSettings) | Esegui il rendering della cartella di lavoro sulla stampante |
| [ToPrinter](../../aspose.cells.rendering/workbookrender/toprinter/#toprinter_2)(string) | Esegui il rendering della cartella di lavoro sulla stampante |
| [ToPrinter](../../aspose.cells.rendering/workbookrender/toprinter/#toprinter_1)(PrinterSettings, string) | Esegui il rendering della cartella di lavoro sulla stampante |
| [ToPrinter](../../aspose.cells.rendering/workbookrender/toprinter/#toprinter_4)(string, string) | Esegui il rendering della cartella di lavoro sulla stampante |
| [ToPrinter](../../aspose.cells.rendering/workbookrender/toprinter/#toprinter_3)(string, int, int) | (**Obsoleto.**) Esegui il rendering della cartella di lavoro sulla stampante |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingClassWorkbookRenderDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio e imposta la dimensione della pagina
            worksheet.Cells["A1"].PutValue("Workbook Render Demo");
            worksheet.PageSetup.PaperSize = PaperSizeType.PaperLetter;

            // Crea opzioni immagine
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            
            // Crea il rendering della cartella di lavoro e ottieni la dimensione della pagina
            WorkbookRender render = new WorkbookRender(workbook, options);
            float[] pageSize = render.GetPageSizeInch(0);
            
            // Restituisci i risultati
            Console.WriteLine($"Page Width: {pageSize[0]} inches");
            Console.WriteLine($"Page Height: {pageSize[1]} inches");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


