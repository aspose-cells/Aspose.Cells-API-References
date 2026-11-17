---
title: "CellValueFormatStrategy Enum"
linktitle: "CellValueFormatStrategy"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "CellValueFormatStrategy enum. Incapsula l'oggetto che rappresenta cellvalueformatstrategy in Go."
type: docs
weight: 200
url: /it/go-cpp/cellvalueformatstrategy/
---

## CellValueFormatStrategy Enum

Specifica come applicare lo stile al valore della cella.

```go

type CellValueFormatStrategy int32


```

## Campi

| Campo | Descrizione |
| --- | --- |
| [None](./none/) | Non formattato. |
| [CellStyle](./cellstyle/) | Formattato solo con lo stile originale della cella. |
| [DisplayStyle](./displaystyle/) | Formattato con lo stile visualizzato della cella. |
| [DisplayString](./displaystring/) | Ottiene la stringa visualizzata in MS Excel. La principale differenza rispetto a <see cref="DisplayStyle"/> è che questa opzione considera anche l'effetto della larghezza della colonna. Se la larghezza della colonna è troppo piccola per mostrare completamente la stringa formattata, può essere visualizzato "#", proprio come fa MS Excel. |
