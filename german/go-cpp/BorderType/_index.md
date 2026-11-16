---
title: "BorderType Enum"
linktitle: "BorderType"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "BorderType-Enum. Kapselt das Objekt, das den Bordertyp in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/bordertype/
---

## BorderType Enum

Enumeriert die Typen von Randlinien und Diagonallinien.

```go

type BorderType int32


```

## Felder

| Feld | Beschreibung |
| --- | --- |
| [LeftBorder](./leftborder/) | Stellt die linke Rahmenlinie dar. |
| [RightBorder](./rightborder/) | Stellt die rechte Rahmenlinie dar, falls vorhanden. |
| [TopBorder](./topborder/) | Stellt die obere Rahmenlinie dar. |
| [BottomBorder](./bottomborder/) | Stellt die untere Rahmenlinie dar. |
| [DiagonalDown](./diagonaldown/) | Stellt die diagonale Linie von oben links nach unten rechts dar. |
| [DiagonalUp](./diagonalup/) | Stellt die diagonale Linie von unten links nach oben rechts dar. |
| [Vertical](./vertical/) | Nur für dynamische Stile, wie bedingte Formatierung, Pivot‑Tabelle. |
| [Horizontal](./horizontal/) | Nur für dynamische Stile, wie bedingte Formatierung, Pivot‑Tabelle. |
| [SideBorders](./sideborders/) | Gibt die vier Seitenränder an: <see cref=\"LeftBorder\"/>,<see cref=\"RightBorder\"/>, <see cref=\"TopBorder\"/> und <see cref=\"BottomBorder\"/>. |
| [Diagonal](./diagonal/) | Spezielle Kombination mehrerer Rahmen zum Komfort des Benutzers für einige APIs. Gibt die diagonalen Rahmen von <see cref=\"DiagonalUp\"/> und <see cref=\"DiagonalDown\"/> an. |
| [DynamicStyleBorders](./dynamicstyleborders/) | Gibt <see cref=\"Vertical\"/> und <see cref=\"Horizontal\"/> des dynamischen Stils an. |
| [None](./none/) | Es wurde kein Rahmen angegeben. |
