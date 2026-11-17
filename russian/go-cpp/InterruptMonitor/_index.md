---
title: "Класс InterruptMonitor"
linktitle: "InterruptMonitor"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс InterruptMonitor. Инкапсулирует объект, представляющий interruptmonitor в Go."
type: docs
weight: 200
url: /ru/go-cpp/interruptmonitor/
---

## InterruptMonitor class

Представляет все операторы, связанные с прерыванием.

```go

type InterruptMonitor struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |
| [NewInterruptMonitor](./newinterruptmonitor/) | Конструктор по умолчанию. |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [IsInterruptionRequested](./isinterruptionrequested/) | Отметить монитор как запрашивающий прерывание |
| [Interrupt](./interrupt/) | Прервать текущий оператор. |
