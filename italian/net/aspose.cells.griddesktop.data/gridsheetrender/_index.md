---
title: "Classe GridSheetRender"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.GridDesktop.Data.GridSheetRender classe. Rappresenta un rendering di foglio di lavoro che può renderizzare il foglio in varie immagini come BMP, PNG, JPEG, TIFF... Il costruttore di questa classe deve essere usato dopo la modifica dello stile della cella di impostazione pagina"
type: docs
url: /it/net/aspose.cells.griddesktop.data/gridsheetrender/
---
## GridSheetRender class

Rappresenta il rendering di un foglio di lavoro che può renderizzare il foglio in varie immagini come (BMP, PNG, JPEG, TIFF...). Il costruttore di questa classe deve essere utilizzato dopo la modifica di pagesetup e dello stile delle celle.

```csharp
public class GridSheetRender
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [GridSheetRender](gridsheetrender/)(Worksheet, GridImageOrPrintOptions) | la costruzione di SheetRender, richiede foglio di lavoro e ImageOrPrintOptions come parametri |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [PageCount](../../aspose.cells.griddesktop.data/gridsheetrender/pagecount/) { get; } | Restituisce il conteggio totale delle pagine del foglio di lavoro corrente. |
| [PageScale](../../aspose.cells.griddesktop.data/gridsheetrender/pagescale/) { get; } | Restituisce la scala di pagina calcolata del foglio. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [GetPageSizeInch](../../aspose.cells.griddesktop.data/gridsheetrender/getpagesizeinch/)(int) | Ottieni la dimensione della pagina in pollici dell'immagine di output. |
| [ToImage](../../aspose.cells.griddesktop.data/gridsheetrender/toimage/#toimage)(int) | Esegui il rendering di una pagina specifica in un oggetto Bitmap. |
| [ToImage](../../aspose.cells.griddesktop.data/gridsheetrender/toimage/#toimage_3)(int, Stream) | Esegui il rendering di una pagina specifica in uno stream. |
| [ToImage](../../aspose.cells.griddesktop.data/gridsheetrender/toimage/#toimage_4)(int, string) | Esegui il rendering di una pagina specifica in un file. |
| [ToImage](../../aspose.cells.griddesktop.data/gridsheetrender/toimage/#toimage_1)(int, Graphics, float, float) | Renderizza una certa pagina su un oggetto Graphics |
| [ToImage](../../aspose.cells.griddesktop.data/gridsheetrender/toimage/#toimage_2)(int, Graphics, float, float, float, float) | Renderizza una certa pagina su un oggetto Graphics |
| [ToPrinter](../../aspose.cells.griddesktop.data/gridsheetrender/toprinter/#toprinter)(PrinterSettings) | Renderizza il foglio di lavoro sulla stampante |
| [ToPrinter](../../aspose.cells.griddesktop.data/gridsheetrender/toprinter/#toprinter_2)(string) | Renderizza il foglio di lavoro sulla stampante |
| [ToPrinter](../../aspose.cells.griddesktop.data/gridsheetrender/toprinter/#toprinter_1)(PrinterSettings, string) | Renderizza il foglio di lavoro sulla stampante |
| [ToPrinter](../../aspose.cells.griddesktop.data/gridsheetrender/toprinter/#toprinter_3)(string, string) | Renderizza il foglio di lavoro sulla stampante |
| [ToTiff](../../aspose.cells.griddesktop.data/gridsheetrender/totiff/#totiff)(Stream) | Renderizza l'intero foglio di lavoro come immagine Tiff nello stream. |
| [ToTiff](../../aspose.cells.griddesktop.data/gridsheetrender/totiff/#totiff_1)(string) | Renderizza l'intero foglio di lavoro come immagine Tiff in un file. |

### Vedi anche

* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


