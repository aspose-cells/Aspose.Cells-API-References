---
title: "HyperlinkLoadMode Enum"
linktitle: "HyperlinkLoadMode"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "HyperlinkLoadMode enum. Incapsula l'oggetto che rappresenta hyperlinkloadmode in Go."
type: docs
weight: 200
url: /it/go-cpp/hyperlinkloadmode/
---

## HyperlinkLoadMode Enum

Specifica come vengono gestiti i collegamenti ipertestuali durante il caricamento di HTML.

```go

type HyperlinkLoadMode int32


```

## Campi

| Campo | Descrizione |
| --- | --- |
| [Normal](./normal/) | Viene caricato solo il primo collegamento ipertestuale in una cella, i successivi vengono ignorati. |
| [AllowMultiple](./allowmultiple/) | Tutti i collegamenti ipertestuali in una cella vengono aggiunti a <see cref="Worksheet.Hyperlinks"/>.Nota che MS Excel supporta solo un collegamento ipertestuale per cella, quindi questa opzione potrebbe produrre file che Excel non può rendere completamente. |
