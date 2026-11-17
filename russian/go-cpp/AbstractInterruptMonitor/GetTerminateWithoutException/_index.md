---
title: "GetTerminateWithoutException метод"
linktitle: "GetTerminateWithoutException"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "GetTerminateWithoutException метод. Инкапсулирует функцию, представляющую getterminatewithoutexception в Go."
type: docs
weight: 200
url: /ru/go-cpp/abstractinterruptmonitor/getterminatewithoutexception/
---

## GetTerminateWithoutException function

Когда процедура прерывается, следует ли тихо завершать её или бросать исключение. По умолчанию false, то есть когда IsInterruptionRequested равно true, будет выброшено CellsException с кодом ExceptionType.Interrupted.

```go

func (instance *AbstractInterruptMonitor) GetTerminateWithoutException()  (bool,  error) 

```

## Примечания


## См. также

* Class [AbstractInterruptMonitor](../)
* Library [Aspose.Cells for Go](../../)
