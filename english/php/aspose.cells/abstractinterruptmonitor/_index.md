---
title: "AbstractInterruptMonitor Class"
linktitle: "AbstractInterruptMonitor"
articleTitle: "AbstractInterruptMonitor"
second_title: "Aspose.Cells for PHP via Java"
description: "Monitor for interruption requests in all time-consuming operations."
type: docs
weight: 50
url: /php/aspose.cells/abstractinterruptmonitor/
---

## AbstractInterruptMonitor class

Monitor for interruption requests in all time-consuming operations.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [IsInterruptionRequested](#isinterruptionrequested) | boolean | Indicates whether interruption is requested for current operation. If true then current operation will be interrupted. I |
| [TerminateWithoutException](#terminatewithoutexception) | boolean | When procedure is interrupted, whether terminate the procedure quietly or throw an Exception. Default is false, that is, |

### AbstractInterruptMonitor.IsInterruptionRequested property {#isinterruptionrequested}

Indicates whether interruption is requested for current operation. If true then current operation will be interrupted. Implementation should perform fast and efficient check here, otherwise it may become another bottleneck for the procedure.

**Type:** boolean

### AbstractInterruptMonitor.TerminateWithoutException property {#terminatewithoutexception}

When procedure is interrupted, whether terminate the procedure quietly or throw an Exception. Default is false, that is, when IsInterruptionRequested is true, a CellsException with code ExceptionType.INTERRUPTED will be thrown.

**Type:** boolean
