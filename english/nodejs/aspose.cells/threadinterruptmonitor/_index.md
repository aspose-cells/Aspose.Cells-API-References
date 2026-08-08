---
title: "ThreadInterruptMonitor"
linktitle: "ThreadInterruptMonitor"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Simple implementation of AbstractInterruptMonitor by starting another thread to require the interruption after sleeping user specified limit."
type: docs
weight: 4200
url: /nodejs/aspose.cells/threadinterruptmonitor/
---

## ThreadInterruptMonitor class

Simple implementation of AbstractInterruptMonitor by starting another thread to require the interruption after sleeping user specified limit. One monitor instance can be used repeatedly, as long as you monitor each process in sequence. It should not be used to monitor multiple procedures concurrently in multi-threads.

```js
new ThreadInterruptMonitor(terminateWithoutException)
```

Constructs one interruption monitor.

## Methods

| Name | Description |
| --- | --- |
| [finishMonitor()](#finishmonitor) | Finishes the monitor for one procedure. Calling this method after the monitored procedure can release the monitor thread |
| [getTerminateWithoutException()](#getterminatewithoutexception) | See TerminateWithoutException. This property is specified by user when constructing this monitor instance. |
| [isInterruptionRequested()](#isinterruptionrequested) | This implementation just checks whether the time cost(from the time when starting this monitor to now) is greater than u |
| [startMonitor(msLimit)](#startmonitor) | Starts the monitor with the specified time limit. The start time to calculate time cost is just when this method is call |

### finishMonitor() {#finishmonitor}

Finishes the monitor for one procedure. Calling this method after the monitored procedure can release the monitor thread earlier, especially when there is no interruption for it(the time cost of that procedure is less than the specified time limit).

### getTerminateWithoutException() {#getterminatewithoutexception}

See TerminateWithoutException. This property is specified by user when constructing this monitor instance.

### isInterruptionRequested() {#isinterruptionrequested}

This implementation just checks whether the time cost(from the time when starting this monitor to now) is greater than user specified limit.

### startMonitor(msLimit) {#startmonitor}

Starts the monitor with the specified time limit. The start time to calculate time cost is just when this method is called, so the procedure which needs to be monitored should be started just after this call.

| Parameter | Type | Description |
| --- | --- | --- |
| msLimit | Number | time limit(ms) to require the interruption. |
