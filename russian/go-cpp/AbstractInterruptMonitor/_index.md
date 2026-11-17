---
title: "Класс AbstractInterruptMonitor"
linktitle: "AbstractInterruptMonitor"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс AbstractInterruptMonitor. Инкапсулирует объект, представляющий abstractinterruptmonitor в Go."
type: docs
weight: 200
url: /ru/go-cpp/abstractinterruptmonitor/
---

## AbstractInterruptMonitor class

Монитор запросов прерывания во всех длительных операциях.

```go

type AbstractInterruptMonitor struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |

## Методы

| Метод | Описание |
| --- | --- |
| [GetTerminateWithoutException](./getterminatewithoutexception/) | Когда процедура прерывается, следует ли тихо завершать её или бросать исключение. По умолчанию false, то есть когда IsInterruptionRequested равно true, будет выброшено CellsException с кодом ExceptionType.Interrupted. |
