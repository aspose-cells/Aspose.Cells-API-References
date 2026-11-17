---
title: "Classe SheetRender"
linktitle: "SheetRender"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe SheetRender. Incapsula l'oggetto che rappresenta sheetrender in Go."
type: docs
weight: 200
url: /it/go-cpp/sheetrender/
---

## SheetRender class

Rappresenta un rendering di foglio di lavoro che può renderizzare il foglio di lavoro in varie immagini come (BMP, PNG, JPEG, TIFF...). Il costruttore di questa classe deve essere utilizzato dopo la modifica di pageSetup e dello stile della cella.

```go

type SheetRender struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewSheetRender](./newsheetrender/) | la costruzione di SheetRender, richiede worksheet e ImageOrPrintOptions come parametri |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetPageCount](./getpagecount/) | Restituisce il conteggio totale delle pagine del foglio di lavoro corrente. |
| [GetPageScale](./getpagescale/) | Restituisce la scala di pagina calcolata del foglio. Restituisce la scala impostata se PageSetup.Zoom è impostato. Altrimenti, restituisce la scala calcolata in base a PageSetup.FitToPagesWide e PageSetup.FitToPagesTall. |
| [GetPageSizeInch](./getpagesizeinch/) | Ottieni le dimensioni della pagina in pollici dell'immagine di output. |
| [ToImage_Int_String](./toimage_int_string/) | Renderizza una determinata pagina su un file. |
| [ToImage_Int](./toimage_int/) | Renderizza una determinata pagina su uno stream. |
| [ToTiff](./totiff/) | Renderizza l'intero foglio di lavoro come immagine Tiff in uno stream. |
| [ToTiff_String](./totiff_string/) | Renderizza l'intero foglio di lavoro come immagine Tiff in un file. |
| [Dispose](./dispose/) | Rilascia le risorse create e utilizzate per il rendering. |
