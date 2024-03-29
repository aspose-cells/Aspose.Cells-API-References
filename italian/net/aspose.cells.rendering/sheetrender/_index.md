---
title: SheetRender
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Rappresenta un rendering di un foglio di lavoro che può eseguire il rendering del foglio di lavoro su varie immagini come BMP PNG JPEG TIFF.. Il costruttore di questa classe deve essere utilizzato dopo la modifica del pagesetup dello stile della cella.
type: docs
weight: 5260
url: /it/net/aspose.cells.rendering/sheetrender/
---
## SheetRender class

Rappresenta un rendering di un foglio di lavoro che può eseguire il rendering del foglio di lavoro su varie immagini come (BMP, PNG, JPEG, TIFF..) Il costruttore di questa classe deve essere utilizzato dopo la modifica del pagesetup, dello stile della cella.

```csharp
public class SheetRender
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [SheetRender](sheetrender)(Worksheet, ImageOrPrintOptions) | il costrutto di SheetRender, necessita di un foglio di lavoro e ImageOrPrintOptions come params |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [PageCount](../../aspose.cells.rendering/sheetrender/pagecount) { get; } | Ottiene il conteggio totale delle pagine del foglio di lavoro corrente. |
| [PageScale](../../aspose.cells.rendering/sheetrender/pagescale) { get; } | Ottiene la scala di pagina calcolata del foglio. Restituisce la scala impostata se[`Zoom`](../../aspose.cells/pagesetup/zoom) è impostato. In caso contrario, restituisce la scala calcolata in base a[`FitToPagesWide`](../../aspose.cells/pagesetup/fittopageswide) e[`FitToPagesTall`](../../aspose.cells/pagesetup/fittopagestall) . |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [CustomPrint](../../aspose.cells.rendering/sheetrender/customprint)(bool, PrintPageEventArgs) | Il client può controllare l'impostazione della pagina della stampante quando stampa ogni pagina utilizzando questa funzione. |
| [GetPageSizeInch](../../aspose.cells.rendering/sheetrender/getpagesizeinch)(int) | Ottieni le dimensioni della pagina in pollici dell'immagine di output. |
| [ToImage](../../aspose.cells.rendering/sheetrender/toimage#toimage)(int) | Rendering di una determinata pagina in un oggetto Bitmap. |
| [ToImage](../../aspose.cells.rendering/sheetrender/toimage#toimage_3)(int, Stream) | Rendering di determinate pagine in uno stream. |
| [ToImage](../../aspose.cells.rendering/sheetrender/toimage#toimage_4)(int, string) | Rendering di determinate pagine in un file. |
| [ToImage](../../aspose.cells.rendering/sheetrender/toimage#toimage_1)(int, Graphics, float, float) | Rendering di determinate pagine in una grafica |
| [ToImage](../../aspose.cells.rendering/sheetrender/toimage#toimage_2)(int, Graphics, float, float, float, float) | Rendering di determinate pagine in una grafica |
| [ToPrinter](../../aspose.cells.rendering/sheetrender/toprinter#toprinter)(PrinterSettings) | Rendering del foglio di lavoro sulla stampante |
| [ToPrinter](../../aspose.cells.rendering/sheetrender/toprinter#toprinter_2)(string) | Rendering del foglio di lavoro sulla stampante |
| [ToPrinter](../../aspose.cells.rendering/sheetrender/toprinter#toprinter_1)(PrinterSettings, string) | Rendering del foglio di lavoro sulla stampante |
| [ToPrinter](../../aspose.cells.rendering/sheetrender/toprinter#toprinter_4)(string, string) | Rendering del foglio di lavoro sulla stampante |
| [ToTiff](../../aspose.cells.rendering/sheetrender/totiff#totiff)(Stream) | Rendering dell'intero foglio di lavoro come immagine Tiff per lo streaming. |
| [ToTiff](../../aspose.cells.rendering/sheetrender/totiff#totiff_1)(string) | Rendering dell'intero foglio di lavoro come immagine Tiff in un file. |

### Guarda anche

* spazio dei nomi [Aspose.Cells.Rendering](../../aspose.cells.rendering)
* assemblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
