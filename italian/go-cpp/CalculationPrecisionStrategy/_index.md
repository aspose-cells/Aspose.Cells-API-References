---
title: "CalculationPrecisionStrategy Enum"
linktitle: "CalculationPrecisionStrategy"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "CalculationPrecisionStrategy enum. Incapsula l'oggetto che rappresenta calculationprecisionstrategy in Go."
type: docs
weight: 200
url: /it/go-cpp/calculationprecisionstrategy/
---

## CalculationPrecisionStrategy Enum

Enumera le strategie per gestire la precisione dei calcoli. A causa del problema di precisione dell'aritmetica floating-point IEEE 754, alcune formule "seemingly simple" potrebbero non essere calcolate come il risultato atteso. Ad esempio la formula "=-0.45+0.43+0.02", calcolando gli operandi con l'operatore '+' direttamente, il risultato non è zero. Per questo tipo di problema di precisione, alcune strategie speciali possono fornire il risultato atteso.

```go

type CalculationPrecisionStrategy int32


```

## Campi

| Campo | Descrizione |
| --- | --- |
| [None](./none/) | Nessuna strategia applicata al calcolo.When calcolando basta usare il valore double originale come operando e restituire direttamente il risultato.Molto efficiente per le prestazioni e applicabile nella maggior parte dei casi. |
| [Round](./round/) | Arrotonda il risultato del calcolo in base alle cifre significative. |
| [Decimal](./decimal/) | Utilizza decimal come operandi quando possibile.Molto inefficiente per le prestazioni. |
