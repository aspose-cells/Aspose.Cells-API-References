---
title: "RowCollection Classe"
linktitle: "RowCollection"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "RowCollection classe. Incapsula l'oggetto che rappresenta rowcollection in Go."
type: docs
weight: 200
url: /it/go-cpp/rowcollection/
---

## RowCollection class

Raccoglie gli oggetti <see cref="Row"/> che rappresentano le singole righe in un foglio di lavoro.

```go

type RowCollection struct  {
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
| [GetCount](./getcount/) | Ottiene il numero di righe in questa collezione. |
| [GetEnumerator](./getenumerator/) | Ottiene un enumeratore che itera le righe attraverso questa collezione |
| [GetEnumerator_Bool_Bool](./getenumerator_bool_bool/) | Ottiene un enumeratore che itera le righe attraverso questa collezione |
| [GetRowByIndex](./getrowbyindex/) | Ottiene l'oggetto riga per la posizione nella lista. |
| [Get](./get/) | Ottiene un oggetto Row per l'indice di riga fornito. L'oggetto Row dell'indice di riga fornito verrà istanziato se non esiste già. |
| [Clear](./clear/) | Cancella tutte le righe e le celle. |
| [RemoveAt](./removeat/) | Rimuove l'elemento riga all'indice (posizione) specificato in questa collezione. |
