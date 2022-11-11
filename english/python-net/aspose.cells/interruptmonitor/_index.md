---
title: InterruptMonitor
second_title: Aspose.Cells for Python via .NET API Reference
description: 
type: docs
weight: 950
url: /python-net/aspose.cells/interruptmonitor/
---

## InterruptMonitor class

Represents all operator about the interrupt.

The InterruptMonitor type exposes the following members:
## Constructors
| Name | Description |
| :- | :- |
|InterruptMonitor()|Initializes a new instance of the InterruptMonitor class|
## Properties
| Name | Description |
| :- | :- |
|is_interruption_requested|Mark the monitor as requesting interruption|
|terminate_without_exception|When procedure is interrupted, whether terminate the procedure quietly or throw an Exception.<br/>            Default is false, that is, when [is_interruption_requested](/python-net/aspose.cells/abstractinterruptmonitor/) is true,<br/>            a [CellsException](/python-net/aspose.cells/cellsexception/) with code [INTERRUPTED](/python-net/aspose.cells/exceptiontype/) will be thrown.|
## Methods
| Name | Description |
| :- | :- |
|interrupt()|Interrupt the current operator.|

### See Also

* namespace [aspose.cells](/python-net/aspose.cells/)
* assembly [Aspose.Cells](/python-net/)

