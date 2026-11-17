---
title: "DrawObject Classe"
linktitle: "DrawObject"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "DrawObject class. Incapsula l'oggetto che rappresenta drawobject in Go."
type: docs
weight: 200
url: /it/go-cpp/drawobject/
---

## DrawObject class

DrawObject verrà inizializzato e restituito durante il rendering.

```go

type DrawObject struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetCell](./getcell/) | Indica l'oggetto Cell durante il rendering.Tutte le proprietà della cella possono essere accedute. |
| [GetShape](./getshape/) | Indica l'oggetto Shape durante il rendering.Tutte le proprietà della forma possono essere accedute. |
| [GetImageBytes](./getimagebytes/) | Indica i byte dell'immagine del Chart e della Shape renderizzati durante il rendering. |
| [GetType](./gettype/) | Indica il tipo di DrawObject. |
| [GetCurrentPage](./getcurrentpage/) | Indica l'indice di pagina di DrawObject.L'indice di pagina parte da zero.Un foglio contiene diverse pagine durante il rendering. |
| [GetTotalPages](./gettotalpages/) | Indica il numero totale di pagine nel rendering corrente. |
| [GetSheetIndex](./getsheetindex/) | Indica l'indice del foglio corrente di DrawObject. |
