---
title: "ConditionalFormattingValue klass"
linktitle: "ConditionalFormattingValue"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "ConditionalFormattingValue klass. Inkapslar objektet som representerar conditionalformattingvalue i Go."
type: docs
weight: 200
url: /sv/go-cpp/conditionalformattingvalue/
---

## ConditionalFormattingValue class

Beskriver värdena för interpolationspunkterna i en gradientskala, dataBar eller iconSet.

```go

type ConditionalFormattingValue struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [GetValue](./getvalue/) | Hämta eller ange värdet för detta villkorliga formateringsvärde‑objekt. Det bör användas tillsammans med Type. |
| [SetValue](./setvalue/) | Hämta eller ange värdet för detta villkorliga formateringsvärde‑objekt. Det bör användas tillsammans med Type. |
| [GetType](./gettype/) | Hämta eller ange typen för detta villkorliga formateringsvärde‑objekt. Genom att sätta typen till FormatConditionValueType.Min eller FormatConditionValueType.Max sätts automatiskt "Value" till null. |
| [SetType](./settype/) | Hämta eller ange typen för detta villkorliga formateringsvärde‑objekt. Genom att sätta typen till FormatConditionValueType.Min eller FormatConditionValueType.Max sätts automatiskt "Value" till null. |
| [IsGTE](./isgte/) | Hämta eller ange flaggan Greater Than Or Equal. Använd endast för ikonsätt, bestämmer om detta tröskelvärde använder operatorn större än eller lika med. 'false' indikerar att 'greater than' används istället för 'greater than or equal to'. Standardvärdet är true. |
| [SetIsGTE](./setisgte/) | Hämta eller ange flaggan Greater Than Or Equal. Använd endast för ikonsätt, bestämmer om detta tröskelvärde använder operatorn större än eller lika med. 'false' indikerar att 'greater than' används istället för 'greater than or equal to'. Standardvärdet är true. |
