---
title: "MergedCellsShrinkType Enum"
linktitle: "MergedCellsShrinkType"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "MergedCellsShrinkType Enum. Kapselt das Objekt, das mergedcellsshrinktype in Go repräsentiert."
type: docs
weight: 200
url: /de/go-cpp/mergedcellsshrinktype/
---

## MergedCellsShrinkType Enum

Stellt die Strategie zum Verkleinern zusammengeführter Zellen für Vorgänge wie das Löschen leerer Zeilen/Spalten dar.

```go

type MergedCellsShrinkType int32


```

## Felder

| Feld | Beschreibung |
| --- | --- |
| [None](./none/) | Lässt die zusammengeführten Zellen unverändert, ohne Änderungen. |
| [ShrinkToFit](./shrinktofit/) | Verkleinert den zusammengeführten Bereich bei Bedarf, indem Zeilen von unten oder Spalten von rechts entfernt werden, während sichergestellt wird, dass alle Inhalte sichtbar bleiben. |
| [KeepHeaderOnly](./keepheaderonly/) | Behält nur die Kopfzeilen/Spalten des zusammengeführten Bereichs, wenn die obere linke Zelle des zusammengeführten Bereichs nicht leer ist. |
