---
title: "ThreadInterruptMonitor Class"
linktitle: "ThreadInterruptMonitor"
articleTitle: "ThreadInterruptMonitor"
second_title: "Aspose.Cells for Python via Java"
description: "Simple implementation of AbstractInterruptMonitor by starting another thread to require the interruption after sleeping user specified limit."
type: docs
weight: 6870
url: /python-java/asposecells.api/threadinterruptmonitor/
---

## ThreadInterruptMonitor class

Simple implementation of AbstractInterruptMonitor by starting another thread to require the interruption after sleeping user specified limit.

## Constructors

| Name | Description |
| --- | --- |
| [ThreadInterruptMonitor](#constructor) | Constructs one interruption monitor. |

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [IsInterruptionRequested](#isinterruptionrequested) | boolean | This implementation just checks whether the time cost(from the time when starting this monitor to now) is greater than u |
| [TerminateWithoutException](#terminatewithoutexception) | boolean | See TerminateWithoutException . This property is specified by user when constructing this monitor instance. |

## Methods

| Name | Description |
| --- | --- |
| [startMonitor](#startmonitor) | Starts the monitor with the specified time limit. The start time to calculate time cost is just when this method is call |
| [finishMonitor](#finishmonitor) | Finishes the monitor for one procedure.

Calling this method after the monitored procedure can release the monitor threa |

### ThreadInterruptMonitor(terminateWithoutException) {#constructor}

Constructs one interruption monitor.

| Parameter | Type | Description |
| --- | --- | --- |
| terminateWithoutException | boolean | TerminateWithoutException |

### ThreadInterruptMonitor.IsInterruptionRequested property {#isinterruptionrequested}

This implementation just checks whether the time cost(from the time when starting this monitor to now) is greater than user specified limit.

**Type:** boolean

### ThreadInterruptMonitor.TerminateWithoutException property {#terminatewithoutexception}

See TerminateWithoutException . This property is specified by user when constructing this monitor instance.

**Type:** boolean

### startMonitor(msLimit) {#startmonitor}

Starts the monitor with the specified time limit. The start time to calculate time cost is just when this method is called, so the procedure which needs to be monitored should be started just after this call.

| Parameter | Type | Description |
| --- | --- | --- |
| msLimit | int | time limit(ms) to require the interruption. |

### finishMonitor() {#finishmonitor}

Finishes the monitor for one procedure.

Calling this method after the monitored procedure can release the monitor thread earlier, especially when there is no interruption for it(the time cost of that procedure is less than the specified time limit).
