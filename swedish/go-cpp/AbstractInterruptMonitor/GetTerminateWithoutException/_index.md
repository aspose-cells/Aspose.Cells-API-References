---
title: "GetTerminateWithoutException Metod"
linktitle: "GetTerminateWithoutException"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "GetTerminateWithoutException metod. Inkapslar funktionen som representerar getterminatewithoutexception i Go."
type: docs
weight: 200
url: /sv/go-cpp/abstractinterruptmonitor/getterminatewithoutexception/
---

## GetTerminateWithoutException function

När proceduren avbryts, om den ska avslutas tyst eller kasta ett undantag. Standard är falskt, det vill säga när IsInterruptionRequested är true, kommer ett CellsException med kod ExceptionType.Interrupted att kastas.

```go

func (instance *AbstractInterruptMonitor) GetTerminateWithoutException()  (bool,  error) 

```

## Anmärkningar


## Se även

* Class [AbstractInterruptMonitor](../)
* Library [Aspose.Cells for Go](../../)
