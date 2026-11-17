---
title: "Classe ColumnCollection"
linktitle: "ColumnCollection"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe ColumnCollection. Incapsula l'oggetto che rappresenta columncollection in Go."
type: docs
weight: 200
url: /it/go-cpp/columncollection/
---

## ColumnCollection class

Raccolta degli oggetti <see cref=\"Column\"/> che rappresentano le singole colonne (impostazioni) in un foglio di lavoro. L'oggetto Column rappresenta solo le impostazioni come larghezza della colonna, stili, ecc. per l'intera colonna, non ha nulla a che fare con la presenza o meno di celle non vuote (dati) nella colonna corrispondente. E il \"Count\" di questa raccolta rappresenta solo il numero di oggetti Column che sono stati istanziati in questa raccolta, non ha nulla a che fare con la presenza o meno di celle non vuote (dati) nel foglio di lavoro.

```go

type ColumnCollection struct  {
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
| [GetColumnByIndex](./getcolumnbyindex/) | Ottiene l'oggetto Column in base alla posizione nell'elenco. |
| [Get](./get/) | Ottiene un oggetto Column per indice di colonna. L'oggetto Column dell'indice di colonna specificato verrà istanziato se non esiste già. |
| [GetCount](./getcount/) | Ottiene il numero di elementi contenuti nell'istanza. |
