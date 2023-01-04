---
title: InterruptMonitor class
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 950
url: /python-net/aspose.cells/interruptmonitor/
is_root: false
---

## InterruptMonitor class

Represents all operator about the interrupt.



**Inheritance:** [InterruptMonitor](/cells/python-net/aspose.cells/interruptmonitor) → 
[AbstractInterruptMonitor](/cells/python-net/aspose.cells/abstractinterruptmonitor)



The InterruptMonitor type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [InterruptMonitor()](/cells/python-net/aspose.cells/interruptmonitor/__init__/#) | Constructs a new instance of InterruptMonitor |


### Properties
| Property | Description |
| :- | :- |
| [is_interruption_requested](/cells/python-net/aspose.cells/interruptmonitor/is_interruption_requested) | Mark the monitor as requesting interruption |
| [terminate_without_exception](/cells/python-net/aspose.cells/interruptmonitor/terminate_without_exception) | When procedure is interrupted, whether terminate the procedure quietly or throw an Exception.<br/>Default is false, that is, when [AbstractInterruptMonitor.is_interruption_requested](/cells/python-net/aspose.cells/abstractinterruptmonitor#is_interruption_requested) is true,<br/>a [CellsException](/cells/python-net/aspose.cells/cellsexception) with code [ExceptionType.INTERRUPTED](/cells/python-net/aspose.cells/exceptiontype#INTERRUPTED) will be thrown. |


### Methods
| Method | Description |
| :- | :- |
| [interrupt()](/cells/python-net/aspose.cells/interruptmonitor/interrupt/#) | Interrupt the current operator. |


### See Also

* module [aspose.cells](../)
* class [AbstractInterruptMonitor](/cells/python-net/aspose.cells/abstractinterruptmonitor)
