---
title: "Enum MergeEmptyTdType"
linktitle: "MergeEmptyTdType"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Enum MergeEmptyTdType. Incapsula l'oggetto che rappresenta mergeemptytdtype in Go."
type: docs
weight: 200
url: /it/go-cpp/mergeemptytdtype/
---

## MergeEmptyTdType Enum

Rappresenta il tipo di unione per un elemento TD vuoto durante l'esportazione di un file in HTML.

```go

type MergeEmptyTdType int32


```

## Campi

| Campo | Descrizione |
| --- | --- |
| [Default](./default/) | Visualizza come MS Excel. |
| [None](./none/) | Gli elementi TD vuoti non verranno uniti durante l'esportazione del file in HTML. Questo genererà un file HTML notevolmente più grande. |
| [MergeForcely](./mergeforcely/) | Unire forzatamente gli elementi TD vuoti durante l'esportazione del file in HTML. La dimensione del file HTML sarà ridotta notevolmente impostando il valore su true. Se desideri importare il file HTML in Excel o esportare linee di griglia perfette quando salvi il file in HTML, mantieni il valore predefinito. |
