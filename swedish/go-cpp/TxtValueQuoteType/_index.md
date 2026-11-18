---
title: "TxtValueQuoteType Enum"
linktitle: "TxtValueQuoteType"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "TxtValueQuoteType enum. Inkapslar objektet som representerar txtvaluequotetype i Go."
type: docs
weight: 200
url: /sv/go-cpp/txtvaluequotetype/
---

## TxtValueQuoteType Enum

Specificerar typen av användning av citattecken för värden i textformatfiler.

```go

type TxtValueQuoteType int32


```

## Fält

| Fält | Beskrivning |
| --- | --- |
| [Normal](./normal/) | Alla värden som innehåller specialtecken såsom citattecken, separator-tecken kommer att omges av citattecken. Samma som beteendet i MS Excel för export av textfil. |
| [Always](./always/) | Alla värden kommer alltid att omges av citattecken. |
| [Minimum](./minimum/) | Citattecken används endast när det behövs. Till exempel, om ett värde innehåller citattecken men citattecknet inte är i början av värdet, kommer detta värde inte att omges av citattecken. |
| [Never](./never/) | Inga värden kommer att omges av citattecken. Den exporterade textfilen med denna typ kanske inte kan läsas korrekt tillbaka eftersom nödvändiga citattecken saknas. |
