---
title: "AbstractInterruptMonitor klass"
linktitle: "AbstractInterruptMonitor"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "AbstractInterruptMonitor klass. Inkapslar objektet som representerar abstractinterruptmonitor i Go."
type: docs
weight: 200
url: /sv/go-cpp/abstractinterruptmonitor/
---

## AbstractInterruptMonitor class

Övervaka avbrottsförfrågningar i alla tidskrävande operationer.

```go

type AbstractInterruptMonitor struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [GetTerminateWithoutException](./getterminatewithoutexception/) | När proceduren avbryts, om den ska avslutas tyst eller kasta ett undantag. Standard är falskt, det vill säga när IsInterruptionRequested är true, kommer ett CellsException med kod ExceptionType.Interrupted att kastas. |
