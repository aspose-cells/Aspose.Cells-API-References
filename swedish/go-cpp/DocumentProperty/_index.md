---
title: "DocumentProperty-klass"
linktitle: "DocumentProperty"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "DocumentProperty-klass. Inkapslar objektet som representerar documentproperty i Go."
type: docs
weight: 200
url: /sv/go-cpp/documentproperty/
---

## DocumentProperty class

Representerar en anpassad eller inbyggd dokumentegenskap.

```go

type DocumentProperty struct  {
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
| [GetName](./getname/) | Returnerar egenskapens namn. |
| [GetValue](./getvalue/) | Hämtar eller anger värdet på egenskapen. |
| [SetValue](./setvalue/) | Hämtar eller anger värdet på egenskapen. |
| [IsLinkedToContent](./islinkedtocontent/) | Indikerar om denna egenskap är länkad till innehåll |
| [GetSource](./getsource/) | Den länkade innehållskällan. |
| [GetType](./gettype/) | Hämtar datatypen för egenskapen. |
| [IsGeneratedName](./isgeneratedname/) | Returnerar true om denna egenskap inte har ett namn i OLE2-lagringen och ett unikt namn genererades endast för det offentliga API:t. |
| [ToString](./tostring/) | Returnerar egenskapsvärdet som en sträng. |
| [ToInt](./toint/) | Returnerar egenskapsvärdet som ett heltal. |
| [ToDouble](./todouble/) | Returnerar egenskapsvärdet som ett dubbelvärde. |
| [ToDateTime](./todatetime/) | Returnerar egenskapsvärdet som DateTime i lokal tidszon. |
| [ToBool](./tobool/) | Returnerar egenskapsvärdet som bool. |
