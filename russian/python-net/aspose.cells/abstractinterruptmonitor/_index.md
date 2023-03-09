---
title: AbstractInterruptMonitor класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 50
url: /ru/python-net/aspose.cells/abstractinterruptmonitor/
is_root: false
---
##  AbstractInterruptMonitor класс
Отслеживайте запросы на прерывание во всех трудоемких операциях.



Тип AbstractInterruptMonitor предоставляет следующие члены:

###  Характеристики
| Свойство| Описание|
| :- | :- |
| [is_interruption_requested](/cells/ru/python-net/aspose.cells/abstractinterruptmonitor/is_interruption_requested) | Указывает, требуется ли прерывание для текущей операции.<br/>Если true, то текущая операция будет прервана.<br/> Реализация должна выполнять здесь быструю и эффективную проверку, иначе это может стать еще одним узким местом для процедуры.|
| [terminate_without_exception](/cells/ru/python-net/aspose.cells/abstractinterruptmonitor/terminate_without_exception) | Когда процедура прерывается, завершайте процедуру тихо или выбрасывайте исключение.<br/>По умолчанию false, то есть когда [AbstractInterruptMonitor.is_interruption_requested](/cells/ru/python-net/aspose.cells/abstractinterruptmonitor#is_interruption_requested) истинно,<br/> будет выброшен [CellsException](/cells/ru/python-net/aspose.cells/cellsexception) с кодом [ExceptionType.INTERRUPTED](/cells/ru/python-net/aspose.cells/exceptiontype#INTERRUPTED).|



###  Смотрите также
* модуль [aspose.cells](..)
* класс [CellsException](/cells/ru/python-net/aspose.cells/cellsexception)
