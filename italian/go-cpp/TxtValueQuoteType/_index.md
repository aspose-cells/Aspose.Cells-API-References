---
title: "Enumerazione TxtValueQuoteType"
linktitle: "TxtValueQuoteType"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Enumerazione TxtValueQuoteType. Incapsula l'oggetto che rappresenta txtvaluequotetype in Go."
type: docs
weight: 200
url: /it/go-cpp/txtvaluequotetype/
---

## TxtValueQuoteType Enum

Specifica il tipo di utilizzo delle virgolette per i valori nei file di formato testo.

```go

type TxtValueQuoteType int32


```

## Campi

| Campo | Descrizione |
| --- | --- |
| [Normal](./normal/) | Tutti i valori che contengono caratteri speciali come virgolette o caratteri separatori saranno racchiusi tra virgolette.Stesso comportamento di MS Excel per l'esportazione di file di testo. |
| [Always](./always/) | Tutti i valori saranno sempre racchiusi tra virgolette. |
| [Minimum](./minimum/) | Metti le virgolette ai valori solo quando necessario. Ad esempio, se un valore contiene un segno di virgolette ma il segno di virgolette non è all'inizio di questo valore, questo valore non verrà quotato. |
| [Never](./never/) | Tutti i valori non saranno quotati. Il file di testo esportato con questo tipo potrebbe non essere letto correttamente perché le virgolette necessarie sono assenti. |
