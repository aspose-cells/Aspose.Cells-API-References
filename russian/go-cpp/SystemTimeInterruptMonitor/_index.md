---
title: "SystemTimeInterruptMonitor Класс"
linktitle: "SystemTimeInterruptMonitor"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "SystemTimeInterruptMonitor class. Инкапсулирует объект, представляющий systemtimeinterruptmonitor в Go."
type: docs
weight: 200
url: /ru/go-cpp/systemtimeinterruptmonitor/
---

## SystemTimeInterruptMonitor class

Простая реализация <see cref="AbstractInterruptMonitor"/> путем проверки и сравнения текущего системного времени с указанным пользователем ограничением.

```go

type SystemTimeInterruptMonitor struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |
| [NewSystemTimeInterruptMonitor](./newsystemtimeinterruptmonitor/) | Создаёт один монитор прерываний. |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [StartMonitor](./startmonitor/) | Запускает монитор с указанным ограничением времени. Время начала для расчёта затраченного времени фиксируется в момент вызова этого метода, поэтому процедура, которую необходимо мониторить, должна быть запущена сразу после этого вызова. |
| [IsInterruptionRequested](./isinterruptionrequested/) | Эта реализация просто проверяет, превышает ли затраченное время (от момента запуска этого монитора до текущего момента) пользовательский лимит. |
| [GetTerminateWithoutException](./getterminatewithoutexception/) | См. AbstractInterruptMonitor.TerminateWithoutException. Это свойство задаётся пользователем при создании экземпляра этого монитора. |
