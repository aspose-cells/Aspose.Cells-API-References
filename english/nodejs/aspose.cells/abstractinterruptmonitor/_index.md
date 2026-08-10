---
title: "AbstractInterruptMonitor"
linktitle: "AbstractInterruptMonitor"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Monitor for interruption requests in all time-consuming operations."
type: docs
weight: 50
url: /nodejs/aspose.cells/abstractinterruptmonitor/
---

## AbstractInterruptMonitor class

Monitor for interruption requests in all time-consuming operations.

## Methods

| Name | Description |
| --- | --- |
| [getTerminateWithoutException()](#getterminatewithoutexception) | When procedure is interrupted, whether terminate the procedure quietly or throw an Exception. Default is false, that is, |
| [isInterruptionRequested()](#isinterruptionrequested) | Indicates whether interruption is requested for current operation. If true then current operation will be interrupted. I |

### getTerminateWithoutException() {#getterminatewithoutexception}

When procedure is interrupted, whether terminate the procedure quietly or throw an Exception. Default is false, that is, when IsInterruptionRequested is true, a CellsException with code ExceptionType.INTERRUPTED will be thrown.

### isInterruptionRequested() {#isinterruptionrequested}

Indicates whether interruption is requested for current operation. If true then current operation will be interrupted. Implementation should perform fast and efficient check here, otherwise it may become another bottleneck for the procedure.
