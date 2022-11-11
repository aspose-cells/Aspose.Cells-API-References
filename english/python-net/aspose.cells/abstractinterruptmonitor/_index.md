---
title: AbstractInterruptMonitor
second_title: Aspose.Cells for Python via .NET API Reference
description: 
type: docs
weight: 50
url: /python-net/aspose.cells/abstractinterruptmonitor/
---

## AbstractInterruptMonitor class

Monitor for interruption requests in all time-consuming operations.

The AbstractInterruptMonitor type exposes the following members:
## Properties
| Name | Description |
| :- | :- |
|is_interruption_requested|Indicates whether interruption is requested for current operation.<br/>            If true then current operation will be interrupted.<br/>            Implementation should perform fast and efficient check here, otherwise it may become another bottleneck for the procedure.|
|terminate_without_exception|When procedure is interrupted, whether terminate the procedure quietly or throw an Exception.<br/>            Default is false, that is, when [is_interruption_requested](/python-net/aspose.cells/abstractinterruptmonitor/) is true,<br/>            a [CellsException](/python-net/aspose.cells/cellsexception/) with code [INTERRUPTED](/python-net/aspose.cells/exceptiontype/) will be thrown.|

### See Also

* namespace [aspose.cells](/python-net/aspose.cells/)
* assembly [Aspose.Cells](/python-net/)

