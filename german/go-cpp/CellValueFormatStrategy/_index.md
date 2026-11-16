---
title: "CellValueFormatStrategy Enum"
linktitle: "CellValueFormatStrategy"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "CellValueFormatStrategy enum. Kapselt das Objekt, das cellvalueformatstrategy in Go repräsentiert."
type: docs
weight: 200
url: /de/go-cpp/cellvalueformatstrategy/
---

## CellValueFormatStrategy Enum

Gibt an, wie der Stil für den Zellwert angewendet wird.

```go

type CellValueFormatStrategy int32


```

## Felder

| Feld | Beschreibung |
| --- | --- |
| [None](./none/) | Nicht formatiert. |
| [CellStyle](./cellstyle/) | Nur mit dem ursprünglichen Stil der Zelle formatiert. |
| [DisplayStyle](./displaystyle/) | Formatiert mit dem angezeigten Stil der Zelle. |
| [DisplayString](./displaystring/) | Ruft die in MS Excel angezeigte Zeichenkette ab. Der Hauptunterschied zu <see cref=\"DisplayStyle\"/> besteht darin, dass diese Option auch die Auswirkung der Spaltenbreite berücksichtigt. Ist die Spaltenbreite zu klein, um die formatierte Zeichenkette vollständig anzuzeigen, kann \"#\" angezeigt werden, genau wie in MS Excel. |
