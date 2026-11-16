---
title: "HtmlCrossType Aufzählung"
linktitle: "HtmlCrossType"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "HtmlCrossType Aufzählung. Kapselt das Objekt, das htmlcrosstype in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/htmlcrosstype/
---

## HtmlCrossType Enum

Stellt fünf Typen von HTML‑Cross‑String dar.

```go

type HtmlCrossType int32


```

## Felder

| Feld | Beschreibung |
| --- | --- |
| [Default](./default/) | Anzeige wie in MS Excel, abhängig von der nächsten Zelle. Wenn die nächste Zelle null ist, wird die Zeichenkette übergreifend, sonst wird sie abgeschnitten. |
| [MSExport](./msexport/) | Zeigt die Zeichenkette wie in MS Excel beim Exportieren von HTML an. |
| [Cross](./cross/) | Anzeige des HTML‑Kreuz‑Strings, diese Leistung beim Erstellen großer HTML‑Dateien ist mehr als zehnmal schneller als das Setzen des Werts auf Default oder FitToCell. |
| [CrossHideRight](./crosshideright/) | Anzeige des HTML‑Kreuz‑Strings und Ausblenden des rechten Strings, wenn sich die Texte überlappen. |
| [FitToCell](./fittocell/) | Nur die Zeichenkette innerhalb der Zellbreite anzeigen. |
