---
title: "MergeEmptyTdType Enum"
linktitle: "MergeEmptyTdType"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "MergeEmptyTdType enum. Kapselt das Objekt, das mergeemptytdtype in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/mergeemptytdtype/
---

## MergeEmptyTdType Enum

Stellt den Zusammenführungs‑Typ für ein leeres TD‑Element beim Export einer Datei nach HTML dar.

```go

type MergeEmptyTdType int32


```

## Felder

| Feld | Beschreibung |
| --- | --- |
| [Default](./default/) | Anzeige wie MS Excel. |
| [None](./none/) | Leere TD-Elemente werden beim Exportieren der Datei nach HTML nicht zusammengeführt. Dies erzeugt eine deutlich größere HTML-Datei. |
| [MergeForcely](./mergeforcely/) | Leere TD-Elemente werden beim Exportieren der Datei nach HTML zwangsweise zusammengeführt. Die Größe der HTML-Datei wird nach dem Setzen des Wertes auf true deutlich reduziert. Wenn Sie die HTML-Datei nach Excel importieren oder beim Speichern der Datei nach HTML perfekte Gitternetzlinien exportieren möchten, behalten Sie den Standardwert bei. |
