---
title: "Classe PivotFieldCollection"
linktitle: "PivotFieldCollection"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe PivotFieldCollection. Incapsula l'oggetto che rappresenta pivotfieldcollection in Go."
type: docs
weight: 200
url: /it/go-cpp/pivotfieldcollection/
---

## PivotFieldCollection class

Rappresenta una raccolta di tutti gli oggetti PivotField nelle diverse regioni della tabella pivot.

```go

type PivotFieldCollection struct  {
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
| [GetType](./gettype/) | Restituisce il tipo PivotFields. |
| [Get_Int](./get_int/) | Restituisce l'oggetto PivotField all'indice specificato. |
| [Get_String](./get_string/) | Restituisce l'oggetto PivotField del nome specifico. |
| [RemoveAt](./removeat/) | Rimuove il campo per indice. Solo per filtro, riga, colonna, regione dati. |
| [AddByBaseIndex](./addbybaseindex/) | Aggiunge un oggetto PivotField al tipo specifico PivotFields. |
| [Add](./add/) | Aggiunge un oggetto PivotField al tipo specifico PivotFields. |
| [Insert](./insert/) | Inserisce un campo pivot all'indice specifico. |
| [Clear](./clear/) | cancella tutti i campi di PivotFieldCollection |
| [Remove](./remove/) | Rimuove il campo dalla regione corrente. |
| [Move](./move/) | Sposta il PivotField dalla posizione corrente alla posizione di destinazione |
| [GetCount](./getcount/) | Ottiene il numero di elementi contenuti nell'istanza. |
