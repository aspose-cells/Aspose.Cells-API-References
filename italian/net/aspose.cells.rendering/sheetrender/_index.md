---
title: "Classe SheetRender"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Rendering.SheetRender. Rappresenta il rendering di un foglio di lavoro che può renderizzare il foglio in varie immagini come BMP, PNG, JPEG, TIFF... Il costruttore di questa classe deve essere usato dopo la modifica dello stile della cella di impostazione pagina"
type: docs
url: /it/net/aspose.cells.rendering/sheetrender/
---
## SheetRender class

Rappresenta il rendering di un foglio di lavoro che può renderizzare il foglio in varie immagini come (BMP, PNG, JPEG, TIFF...). Il costruttore di questa classe deve essere utilizzato dopo la modifica di pagesetup e dello stile delle celle.

```csharp
public class SheetRender
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [SheetRender](sheetrender/)(Worksheet, ImageOrPrintOptions) | la costruzione di SheetRender, richiede foglio di lavoro e ImageOrPrintOptions come parametri |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [PageCount](../../aspose.cells.rendering/sheetrender/pagecount/) { get; } | Restituisce il conteggio totale delle pagine del foglio di lavoro corrente. |
| [PageScale](../../aspose.cells.rendering/sheetrender/pagescale/) { get; } | Restituisce la scala di pagina calcolata del foglio. Restituisce la scala impostata se [`Zoom`](../../aspose.cells/pagesetup/zoom/) è impostato. Altrimenti, restituisce la scala calcolata in base a [`FitToPagesWide`](../../aspose.cells/pagesetup/fittopageswide/) e [`FitToPagesTall`](../../aspose.cells/pagesetup/fittopagestall/). |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [CustomPrint](../../aspose.cells.rendering/sheetrender/customprint/)(bool, PrintPageEventArgs) | Il client può controllare le impostazioni della pagina della stampante quando stampa ogni pagina usando questa funzione. |
| [Dispose](../../aspose.cells.rendering/sheetrender/dispose/)() | Rilascia le risorse create e usate per il rendering. |
| [GetPageSizeInch](../../aspose.cells.rendering/sheetrender/getpagesizeinch/)(int) | Ottieni la dimensione della pagina in pollici dell'immagine di output. |
| [ToImage](../../aspose.cells.rendering/sheetrender/toimage/#toimage)(int) | Esegui il rendering di una pagina specifica in un oggetto Bitmap. |
| [ToImage](../../aspose.cells.rendering/sheetrender/toimage/#toimage_3)(int, Stream) | Esegui il rendering di una pagina specifica in uno stream. |
| [ToImage](../../aspose.cells.rendering/sheetrender/toimage/#toimage_4)(int, string) | Esegui il rendering di una pagina specifica in un file. |
| [ToImage](../../aspose.cells.rendering/sheetrender/toimage/#toimage_1)(int, Graphics, float, float) | Renderizza una certa pagina su un oggetto Graphics |
| [ToImage](../../aspose.cells.rendering/sheetrender/toimage/#toimage_2)(int, Graphics, float, float, float, float) | Renderizza una certa pagina su un oggetto Graphics |
| [ToPrinter](../../aspose.cells.rendering/sheetrender/toprinter/#toprinter)(PrinterSettings) | Renderizza il foglio di lavoro sulla stampante |
| [ToPrinter](../../aspose.cells.rendering/sheetrender/toprinter/#toprinter_2)(string) | Renderizza il foglio di lavoro sulla stampante |
| [ToPrinter](../../aspose.cells.rendering/sheetrender/toprinter/#toprinter_1)(PrinterSettings, string) | Renderizza il foglio di lavoro sulla stampante |
| [ToPrinter](../../aspose.cells.rendering/sheetrender/toprinter/#toprinter_4)(string, string) | Renderizza il foglio di lavoro sulla stampante |
| [ToPrinter](../../aspose.cells.rendering/sheetrender/toprinter/#toprinter_3)(string, int, int) | (**Obsolete.**) Renderizza il foglio di lavoro sulla stampante |
| [ToTiff](../../aspose.cells.rendering/sheetrender/totiff/#totiff)(Stream) | Renderizza l'intero foglio di lavoro come immagine Tiff nello stream. |
| [ToTiff](../../aspose.cells.rendering/sheetrender/totiff/#totiff_1)(string) | Renderizza l'intero foglio di lavoro come immagine Tiff in un file. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingClassSheetRenderDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Aggiungi dati di esempio
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    sheet.Cells[i, j].PutValue($"Data {i},{j}");
                }
            }

            // Configura l'impostazione della pagina
            PageSetup pageSetup = sheet.PageSetup;
            pageSetup.PrintArea = "1:10";
            pageSetup.SetFitToPages(1, 1);

            // Crea SheetRender e dimostra la funzionalità principale
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            SheetRender sr = new SheetRender(sheet, options);
            
            Console.WriteLine($"Number of pages: {sr.PageCount}");
            Console.WriteLine($"Page scale: {sr.PageScale * 100}%");
            
            // Renderizza la prima pagina in immagine (dimostrazione)
            sr.ToImage(0, "output_page1.png");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


