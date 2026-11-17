---
title: "SetHtmlCrossStringType Metodo"
linktitle: "SetHtmlCrossStringType"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "SetHtmlCrossStringType metodo. Incapsula la funzione che rappresenta sethtmlcrossstringtype in Go."
type: docs
weight: 200
url: /it/go-cpp/htmlsaveoptions/sethtmlcrossstringtype/
---

## SetHtmlCrossStringType function

Indica se una stringa che attraversa più celle verrà visualizzata nello stesso modo di MS Excel quando si salva un file Excel in formato html. Per impostazione predefinita il valore è Default, quindi per le stringhe che attraversano più celle c'è poca differenza tra i file html creati da Aspose.Cells e MS Excel. Tuttavia, per le prestazioni nella creazione di file html di grandi dimensioni, impostare il valore su Cross sarebbe diverse volte più veloce rispetto a impostarlo su Default o Fit2Cell.

```go

func (instance *HtmlSaveOptions) SetHtmlCrossStringType(value HtmlCrossType)  error

```

## Osservazioni


## Vedi anche

* Class [HtmlSaveOptions](../)
* Library [Aspose.Cells for Go](../../)
