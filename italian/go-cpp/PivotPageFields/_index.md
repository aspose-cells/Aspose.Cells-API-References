---
title: "Classe PivotPageFields"
linktitle: "PivotPageFields"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "PivotPageFields class. Incapsula l'oggetto che rappresenta pivotpagefields in Go."
type: docs
weight: 200
url: /it/go-cpp/pivotpagefields/
---

## PivotPageFields class

Rappresenta gli elementi della pagina pivot se la fonte dati della tabella pivot è un intervallo di consolidamento. Può contenere fino a 4 elementi.

```go

type PivotPageFields struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewPivotPageFields](./newpivotpagefields/) | Rappresenta gli elementi del campo pagina pivot. |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [AddPageField](./addpagefield/) | Aggiunge un campo pagina. |
| [GetPageFieldCount](./getpagefieldcount/) | Ottiene il numero di campi pagina. |
| [AddIdentify](./addidentify/) | Imposta quale etichetta dell'elemento in ciascun campo pagina utilizzare per identificare l'intervallo di dati. La lunghezza pageItemIndex.Length deve essere uguale a PageFieldCount, quindi aggiungi prima il campo pagina. |
