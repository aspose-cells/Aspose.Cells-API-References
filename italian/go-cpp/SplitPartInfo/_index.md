---
title: "SplitPartInfo Classe"
linktitle: "SplitPartInfo"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "SplitPartInfo classe. Incapsula l'oggetto che rappresenta splitpartinfo in Go."
type: docs
weight: 200
url: /it/go-cpp/splitpartinfo/
---

## SplitPartInfo class

Rappresenta le informazioni di un input/output per più input/output, come la pagina corrente da renderizzare durante la conversione del foglio di calcolo in immagine.

```go

type SplitPartInfo struct  {
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
| [GetPartIndex](./getpartindex/) | Indice della parte corrente nella sequenza (base 0). -1 indica che non ci sono più parti, quindi il risultato è singolo. |
| [GetSheetIndex](./getsheetindex/) | Indice del foglio in cui si trova la parte corrente. -1 indica che c'è un solo foglio. |
| [GetSheetName](./getsheetname/) | Nome del foglio in cui si trova la parte corrente. |
