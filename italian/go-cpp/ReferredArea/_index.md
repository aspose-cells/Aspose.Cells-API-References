---
title: "ReferredArea Classe"
linktitle: "ReferredArea"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "ReferredArea classe. Incapsula l'oggetto che rappresenta referredarea in Go."
type: docs
weight: 200
url: /it/go-cpp/referredarea/
---

## ReferredArea class

Rappresenta un'area di riferimento della formula.

```go

type ReferredArea struct  {
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
| [IsExternalLink](./isexternallink/) | Indica se questo è un collegamento esterno. |
| [GetExternalFileName](./getexternalfilename/) | Ottieni il nome del file esterno se questo è un riferimento esterno. |
| [GetSheetName](./getsheetname/) | Indica in quale foglio si trova questo riferimento. |
| [GetSheetNames](./getsheetnames/) | Nomi di tutti i fogli di lavoro a cui questa istanza fa riferimento. |
| [IsEntireRow](./isentirerow/) | Indica se quest'area contiene tutte le colonne (riga intera). |
| [IsEntireColumn](./isentirecolumn/) | Indica se quest'area contiene tutte le righe (colonna intera). |
| [IsArea](./isarea/) | Indica se questo è un'area. |
| [GetEndColumn](./getendcolumn/) | La colonna finale dell'area. |
| [GetStartColumn](./getstartcolumn/) | La colonna iniziale dell'area. |
| [GetEndRow](./getendrow/) | La riga finale dell'area. |
| [GetStartRow](./getstartrow/) | La riga iniziale dell'area. |
| [GetValues](./getvalues/) | Ottiene i valori delle celle in quest'area. |
| [GetValues_Bool](./getvalues_bool/) | Ottiene i valori delle celle in quest'area. |
| [GetValue_Int_Int](./getvalue_int_int/) | Ottiene il valore della cella con l'offset specificato dall'angolo superiore sinistro di quest'area. |
| [GetValue_Int_Int_Bool](./getvalue_int_int_bool/) | Ottiene il valore della cella con l'offset specificato dall'angolo superiore sinistro di quest'area. |
| [ToString](./tostring/) | Restituisce l'indirizzo di riferimento di quest'area. Generalmente è l'indirizzo del riferimento che può essere usato in una formula, come "Sheet1!A1:C3". |
