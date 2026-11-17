---
title: "Classe PivotItem"
linktitle: "PivotItem"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe PivotItem. Incapsula l'oggetto che rappresenta pivotitem in Go."
type: docs
weight: 200
url: /it/go-cpp/pivotitem/
---

## PivotItem class

Rappresenta un elemento in un report di PivotField.

```go

type PivotItem struct  {
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
| [IsHidden](./ishidden/) | Ottiene e imposta se l'elemento pivot è nascosto. |
| [SetIsHidden](./setishidden/) | Ottiene e imposta se l'elemento pivot è nascosto. |
| [GetPosition](./getposition/) | Specificando l'indice di questo elemento in tutti i PivotItem del campo. |
| [SetPosition](./setposition/) | Specificando l'indice di questo elemento in tutti i PivotItem del campo. |
| [GetPositionInSameParentNode](./getpositioninsameparentnode/) | Specificando l'indice di posizione nei PivotItem sotto lo stesso nodo genitore. |
| [SetPositionInSameParentNode](./setpositioninsameparentnode/) | Specificando l'indice di posizione nei PivotItem sotto lo stesso nodo genitore. |
| [Move](./move/) | Sposta l'elemento su o giù |
| [IsDetailHidden](./isdetailhidden/) | Ottiene e imposta se il dettaglio di questo elemento pivot è nascosto. |
| [SetIsDetailHidden](./setisdetailhidden/) | Ottiene e imposta se il dettaglio di questo elemento pivot è nascosto. |
| [IsCalculatedItem](./iscalculateditem/) | Indica se questo elemento pivot è un elemento di formula calcolata. |
| [GetFormula](./getformula/) | Ottiene la formula di questo elemento calcolato. Funziona solo quando questo elemento è un elemento calcolato. |
| [IsMissing](./ismissing/) | Indica se l'elemento è stato rimosso dalla fonte dati. |
| [GetStringValue](./getstringvalue/) | Ottiene il valore stringa dell'elemento pivot. Se il valore è nullo, restituisce "". |
| [GetDoubleValue](./getdoublevalue/) | Ottiene il valore double dell'elemento pivot. Se il valore è nullo o non è un numero, restituisce 0. |
| [GetDateTimeValue](./getdatetimevalue/) | Ottiene il valore data/ora dell'elemento pivot. Se il valore è nullo, restituisce DateTime.MinValue. |
| [GetValue](./getvalue/) | Ottiene il valore dell'elemento pivot |
| [GetName](./getname/) | Ottiene il nome dell'elemento pivot. |
| [SetName](./setname/) | Ottiene il nome dell'elemento pivot. |
