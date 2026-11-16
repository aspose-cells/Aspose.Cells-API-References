---
title: "CalculationPrecisionStrategy Aufzählung"
linktitle: "CalculationPrecisionStrategy"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "CalculationPrecisionStrategy Aufzählung. Kapselt das Objekt, das calculationprecisionstrategy in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/calculationprecisionstrategy/
---

## CalculationPrecisionStrategy Enum

Enumeriert Strategien zum Umgang mit Berechnungspräzision. Aufgrund von Präzisionsproblemen bei der IEEE‑754-Gleitkommaarithmetik können einige "scheinbar einfache" Formeln nicht das erwartete Ergebnis liefern. Zum Beispiel die Formel "=-0.45+0.43+0.02"; wenn die Operanden direkt mit dem '+'‑Operator berechnet werden, ist das Ergebnis nicht null. Bei solchen Präzisionsproblemen können einige spezielle Strategien das erwartete Ergebnis liefern.

```go

type CalculationPrecisionStrategy int32


```

## Felder

| Feld | Beschreibung |
| --- | --- |
| [None](./none/) | Keine Strategie bei der Berechnung angewendet. Beim Berechnen einfach den ursprünglichen double-Wert als Operand verwenden und das Ergebnis direkt zurückgeben. Am effizientesten für die Leistung und in den meisten Fällen anwendbar. |
| [Round](./round/) | Rundet das Berechnungsergebnis gemäß den signifikanten Stellen. |
| [Decimal](./decimal/) | Verwendet Dezimalzahlen als Operanden, wenn möglich. Am ineffizientesten für die Leistung. |
