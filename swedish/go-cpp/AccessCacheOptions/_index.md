---
title: "AccessCacheOptions enum"
linktitle: "AccessCacheOptions"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "AccessCacheOptions enum. Inkapslar objektet som representerar accesscacheoptions i Go."
type: docs
weight: 200
url: /sv/go-cpp/accesscacheoptions/
---

## AccessCacheOptions Enum

Cache‑alternativ för dataåtkomst. Flera alternativ kan kombineras med hjälp av "|"‑operatorn.

```go

type AccessCacheOptions int32


```

## Fält

| Fält | Beskrivning |
| --- | --- |
| [None](./none/) | Ingen cache för någon dataåtkomst. |
| [All](./all/) | Tillämpa alla möjliga optimeringar för alla typer av dataåtkomst i arbetsboken. Alla inställningar och data får inte ändras under den optimerade åtkomsten. |
| [PositionAndSize](./positionandsize/) | Tillämpa möjlig optimering för att hämta ett objekts (t.ex. Shape) position och storlek. Inställningar för radhöjd och kolumnbredd får inte ändras under den optimerade åtkomsten. |
| [CellsData](./cellsdata/) | Tillämpa möjlig optimering för att hämta cellers värden. Celldata (data och inställningar för Cell, Row) får inte ändras under den optimerade åtkomsten, inga nya Cell/Row-objekt ska heller skapas (t.ex. via <see cref="Cells.this[int, int]"/>). |
| [CellDisplay](./celldisplay/) | Tillämpa möjlig optimering för att hämta displayrelaterade resultat för celler (<see cref="Cell.DisplayStringValue"/>, <see cref="Cell.GetStyle()"/>, <see cref="Cell.GetDisplayStyle()"/>, etc.). Celldata och stilrelaterade objekt (Cell/Row/Column-stilar, kolumnbredd, etc.) får inte ändras under den optimerade åtkomsten. |
| [GetFormula](./getformula/) | Tillämpa möjlig optimering för att hämta formler. All data och inställningar som kan påverka formeluttrycket (arbetsbladets namn, namnens text, tabellens kolumn, etc.) får inte ändras under den optimerade åtkomsten. |
| [SetFormula](./setformula/) | Tillämpa möjlig optimering för att sätta formler. All data och inställningar som kan påverka formeluttrycket (arbetsbladets namn, namnens text, tabellens kolumn, etc.) får inte ändras under den optimerade åtkomsten. |
| [CalculateFormula](./calculateformula/) | Tillämpa möjlig optimering för att beräkna formler. Celldata får inte ändras under den optimerade åtkomsten, inga nya objekt (Cell, Row, etc.) ska heller skapas (t.ex. via <see cref="Cells.this[int, int]"/>). |
| [ConditionalFormatting](./conditionalformatting/) | Tillämpa möjlig optimering för att hämta formateringsresultat för villkorlig formatering. All data och inställningar som kan påverka resultatet av villkorlig formatering (inställningar för villkorlig formatering, beroende cellvärden, etc.) får inte ändras under den optimerade åtkomsten. |
| [Validation](./validation/) | Tillämpa möjlig optimering för att hämta valideringsresultat. All data och inställningar som kan påverka resultatet av validering (inställningar för valideringen, beroende cellvärden, etc.) får inte ändras under den optimerade åtkomsten. |
