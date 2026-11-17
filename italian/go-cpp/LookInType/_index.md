---
title: "Enumerazione LookInType"
linktitle: "LookInType"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "LookInType enumerazione. Incapsula l'oggetto che rappresenta lookintype in Go."
type: docs
weight: 200
url: /it/go-cpp/lookintype/
---

## LookInType Enum

Rappresenta il tipo di look in.

```go

type LookInType int32


```

## Campi

| Campo | Descrizione |
| --- | --- |
| [Formulas](./formulas/) | Trova l'oggetto cercato dalla formula(<see cref="Cell.Formula"/>) se la cella è una formula, altrimenti lo trova dal valore originale della cella (stesso di <see cref="OriginalValues"/>). |
| [Values](./values/) | Trova l'oggetto dal valore originale della cella (<see cref="Cell.Value"/>) e dal valore formattato (<see cref="Cell.StringValue"/>). |
| [ValuesExcludeFormulaCell](./valuesexcludeformulacell/) | Ignora le celle che sono formule. Per quelle celle che non sono formule, è lo stesso di <see cref="Values"/>. |
| [Comments](./comments/) | Trova l'oggetto solo dal commento della cella. Ignora le celle che non hanno commento. |
| [OnlyFormulas](./onlyformulas/) | Ignora le celle che non sono formule. Per quelle celle che sono formule, trova l'oggetto cercato dalla formula (<see cref="Cell.Formula"/>). |
| [OriginalValues](./originalvalues/) | Trova l'oggetto solo dal valore originale della cella. |
| [FormattedValues](./formattedvalues/) | Trova l'oggetto solo dal valore formattato della cella (<see cref="Cell.StringValue"/>). |
