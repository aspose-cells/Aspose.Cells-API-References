---
title: "Classe WorkbookRender"
linktitle: "WorkbookRender"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe WorkbookRender. Incapsula l'oggetto che rappresenta workbookrender in Go."
type: docs
weight: 200
url: /it/go-cpp/workbookrender/
---

## WorkbookRender class

Rappresenta un rendering di cartella di lavoro. Il costruttore di questa classe deve essere utilizzato dopo la modifica di pageSetup e dello stile della cella.

```go

type WorkbookRender struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewWorkbookRender](./newworkbookrender/) | La costruzione di WorkbookRender |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetPageCount](./getpagecount/) | Ottiene il conteggio totale delle pagine della cartella di lavoro. |
| [GetPageSizeInch](./getpagesizeinch/) | Ottieni le dimensioni della pagina in pollici dell'immagine di output. |
| [ToImage](./toimage/) | Renderizza l'intero workbook come immagine Tiff su stream. |
| [ToImage_String](./toimage_string/) | Renderizza l'intero workbook come immagine Tiff su un file. |
| [ToImage_Int_String](./toimage_int_string/) | Renderizza una determinata pagina su un file. |
| [ToImage_Int](./toimage_int/) | Renderizza una determinata pagina su uno stream. |
| [Dispose](./dispose/) | Rilascia le risorse create e utilizzate per il rendering. |
