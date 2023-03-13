---
title: InterruptMonitor класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 950
url: /ru/python-net/aspose.cells/interruptmonitor/
is_root: false
---
##  InterruptMonitor класс
Представляет весь оператор о прерывании.



**Наследование:** [InterruptMonitor](/cells/python-net/aspose.cells/interruptmonitor) → 
[AbstractInterruptMonitor](/cells/ru/python-net/aspose.cells/abstractinterruptmonitor)



Тип InterruptMonitor предоставляет следующие члены:

###  Конструкторы
| Конструктор| Описание|
| :- | :- |
| [InterruptMonitor()](/cells/ru/python-net/aspose.cells/interruptmonitor/__init__/#) | Создает новый экземпляр InterruptMonitor|


###  Характеристики
| Свойство| Описание|
| :- | :- |
| [is_interruption_requested](/cells/ru/python-net/aspose.cells/interruptmonitor/is_interruption_requested) | Пометить монитор как требующий прерывания|
| [terminate_without_exception](/cells/ru/python-net/aspose.cells/interruptmonitor/terminate_without_exception) | Когда процедура прерывается, завершайте процедуру тихо или выбрасывайте исключение.<br/>По умолчанию false, то есть когда [AbstractInterruptMonitor.is_interruption_requested](/cells/ru/python-net/aspose.cells/abstractinterruptmonitor#is_interruption_requested) истинно,<br/> будет выброшен [CellsException](/cells/ru/python-net/aspose.cells/cellsexception) с кодом [ExceptionType.INTERRUPTED](/cells/ru/python-net/aspose.cells/exceptiontype#INTERRUPTED).|


###  Методы
| Метод| Описание|
| :- | :- |
| [interrupt()](/cells/ru/python-net/aspose.cells/interruptmonitor/interrupt/#) | Прервать текущего оператора.|



###  Смотрите также
* модуль [aspose.cells](..)
* класс [AbstractInterruptMonitor](/cells/ru/python-net/aspose.cells/abstractinterruptmonitor)
* класс [CellsException](/cells/ru/python-net/aspose.cells/cellsexception)
* класс [InterruptMonitor](/cells/ru/python-net/aspose.cells/interruptmonitor)
