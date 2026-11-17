---
title: "Classe PivotAreaFilter"
linktitle: "PivotAreaFilter"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe PivotAreaFilter. Incapsula l'oggetto che rappresenta pivotareafilter in Go."
type: docs
weight: 200
url: /it/go-cpp/pivotareafilter/
---

## PivotAreaFilter class

Rappresenta il filtro di <see cref="PivotArea"/> per <see cref="PivotTable"/>.

```go

type PivotAreaFilter struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewPivotAreaFilter](./newpivotareafilter/) | Costruttore predefinito. |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [IsSubtotalSet](./issubtotalset/) | Restituisce quale subtotale è impostato per questo filtro. |
| [SetSubtotals](./setsubtotals/) | Subtotale per il filtro. |
| [GetFieldIndex](./getfieldindex/) | Restituisce l'indice del campo nei campi di origine a cui si riferisce questo filtro.Un valore di -2 indica il campo dei valori. |
| [GetSelected](./getselected/) | Indica se questo campo ha una selezione.Funziona solo quando la tabella pivot è in visualizzazione contorno. |
| [SetSelected](./setselected/) | Indica se questo campo ha una selezione.Funziona solo quando la tabella pivot è in visualizzazione contorno. |
