---
title: AbstractInterruptMonitor class
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 50
url: /python-net/aspose.cells/abstractinterruptmonitor/
is_root: false
---

## AbstractInterruptMonitor class

Monitor for interruption requests in all time-consuming operations.



The AbstractInterruptMonitor type exposes the following members:

### Properties
| Property | Description |
| :- | :- |
| [is_interruption_requested](/cells/python-net/aspose.cells/abstractinterruptmonitor/is_interruption_requested) | Indicates whether interruption is requested for current operation.<br/>If true then current operation will be interrupted.<br/>Implementation should perform fast and efficient check here, otherwise it may become another bottleneck for the procedure. |
| [terminate_without_exception](/cells/python-net/aspose.cells/abstractinterruptmonitor/terminate_without_exception) | When procedure is interrupted, whether terminate the procedure quietly or throw an Exception.<br/>Default is false, that is, when [AbstractInterruptMonitor.is_interruption_requested](/cells/python-net/aspose.cells/abstractinterruptmonitor#is_interruption_requested) is true,<br/>a [CellsException](/cells/python-net/aspose.cells/cellsexception) with code [ExceptionType.INTERRUPTED](/cells/python-net/aspose.cells/exceptiontype#INTERRUPTED) will be thrown. |


### See Also

* module [aspose.cells](../)
