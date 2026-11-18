---
title: "CalculationPrecisionStrategy Enum"
linktitle: "CalculationPrecisionStrategy"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "CalculationPrecisionStrategy enum. Inkapslar objektet som representerar calculationprecisionstrategy i Go."
type: docs
weight: 200
url: /sv/go-cpp/calculationprecisionstrategy/
---

## CalculationPrecisionStrategy Enum

Enumererar strategier för att hantera beräkningsprecision. På grund av precisionsproblemet i IEEE 754 flyttalsaritmetik kan vissa \"verkligen enkla\" formler inte beräknas till det förväntade resultatet. Till exempel formeln \"=-0.45+0.43+0.02\", när operander beräknas med '+'-operatorn direkt, blir resultatet inte noll. För den här typen av precisionsproblem kan vissa speciella strategier ge det förväntade resultatet.

```go

type CalculationPrecisionStrategy int32


```

## Fält

| Fält | Beskrivning |
| --- | --- |
| [None](./none/) | Ingen strategi tillämpas på beräkning. Vid beräkning används bara det ursprungliga dubbelvärdet som operand och resultatet returneras direkt. Mest effektiv för prestanda och tillämplig i de flesta fall. |
| [Round](./round/) | Avrundar beräkningsresultatet enligt signifikanta siffror. |
| [Decimal](./decimal/) | Använder decimal som operander när det är möjligt. Mest ineffektiv för prestanda. |
