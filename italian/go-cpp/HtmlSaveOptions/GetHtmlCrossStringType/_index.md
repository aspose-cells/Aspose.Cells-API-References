---
title: "Metodo GetHtmlCrossStringType"
linktitle: "GetHtmlCrossStringType"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Metodo GetHtmlCrossStringType. Incapsula la funzione che rappresenta gethtmlcrossstringtype in Go."
type: docs
weight: 200
url: /it/go-cpp/htmlsaveoptions/gethtmlcrossstringtype/
---

## GetHtmlCrossStringType function

Indica se una stringa che attraversa più celle verrà visualizzata nello stesso modo di MS Excel quando si salva un file Excel in formato html. Per impostazione predefinita il valore è Default, quindi per le stringhe che attraversano più celle c'è poca differenza tra i file html creati da Aspose.Cells e MS Excel. Tuttavia, per le prestazioni nella creazione di file html di grandi dimensioni, impostare il valore su Cross sarebbe diverse volte più veloce rispetto a impostarlo su Default o Fit2Cell.

```go

func (instance *HtmlSaveOptions) GetHtmlCrossStringType()  (HtmlCrossType,  error) 

```

## Osservazioni


## Vedi anche

* Class [HtmlSaveOptions](../)
* Library [Aspose.Cells for Go](../../)
