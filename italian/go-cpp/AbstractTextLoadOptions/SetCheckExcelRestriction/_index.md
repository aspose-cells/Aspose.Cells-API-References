---
title: "SetCheckExcelRestriction Metodo"
linktitle: "SetCheckExcelRestriction"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "SetCheckExcelRestriction metodo. Incapsula la funzione che rappresenta setcheckexcelrestriction in Go."
type: docs
weight: 200
url: /it/go-cpp/abstracttextloadoptions/setcheckexcelrestriction/
---

## SetCheckExcelRestriction function

Indica se verificare le restrizioni del file Excel quando l'utente modifica oggetti correlati alle celle. Per esempio, Excel non consente l'inserimento di una stringa più lunga di 32K. Quando si inserisce un valore più lungo di 32K, ad esempio tramite Cell.PutValue(string), se questa proprietà è true, si otterrà un'Exception. Se questa proprietà è false, accetteremo la stringa inserita come valore della cella, così in seguito potrai esportare la stringa completa per altri formati di file come CSV. Tuttavia, se hai impostato un valore di questo tipo che è non valido per il formato file Excel, non dovresti salvare la cartella di lavoro come formato Excel in seguito. Altrimenti potrebbero verificarsi errori imprevisti nel file Excel generato.

```go

func (instance *AbstractTextLoadOptions) SetCheckExcelRestriction(value bool)  error

```

## Osservazioni


## Vedi anche

* Class [AbstractTextLoadOptions](../)
* Library [Aspose.Cells for Go](../../)
