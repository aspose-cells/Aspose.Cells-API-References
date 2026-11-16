---
title: "LookInType Aufzählung"
linktitle: "LookInType"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "LookInType Aufzählung. Kapselt das Objekt, das lookintype in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/lookintype/
---

## LookInType Enum

Stellt den 'look in'-Typ dar.

```go

type LookInType int32


```

## Felder

| Feld | Beschreibung |
| --- | --- |
| [Formulas](./formulas/) | Findet das gesuchte Objekt aus der Formel(<see cref="Cell.Formula"/>), wenn die Zelle eine Formel ist, andernfalls aus dem ursprünglichen Wert der Zelle (entspricht <see cref="OriginalValues"/>). |
| [Values](./values/) | Findet das Objekt aus dem ursprünglichen Wert der Zelle(<see cref="Cell.Value"/>) und dem formatierten Wert(<see cref="Cell.StringValue"/>). |
| [ValuesExcludeFormulaCell](./valuesexcludeformulacell/) | Ignoriert Zellen, die Formeln sind. Für diese Zellen, die keine Formeln sind, ist es dasselbe wie <see cref="Values"/>. |
| [Comments](./comments/) | Findet das Objekt nur aus dem Kommentar der Zelle. Ignoriert Zellen, die keinen Kommentar haben. |
| [OnlyFormulas](./onlyformulas/) | Ignoriert Zellen, die keine Formeln sind. Für diese Zellen, die Formeln sind, wird das gesuchte Objekt aus der Formel (<see cref="Cell.Formula"/>) gefunden. |
| [OriginalValues](./originalvalues/) | Findet das Objekt nur aus dem ursprünglichen Wert der Zelle. |
| [FormattedValues](./formattedvalues/) | Findet das Objekt nur aus dem formatierten Wert der Zelle (<see cref="Cell.StringValue"/>). |
