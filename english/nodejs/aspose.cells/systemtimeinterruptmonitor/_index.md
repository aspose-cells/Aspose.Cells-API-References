---
title: "SystemTimeInterruptMonitor"
linktitle: "SystemTimeInterruptMonitor"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Simple implementation of AbstractInterruptMonitor by checking and comparing current system time with user specified limit."
type: docs
weight: 4010
url: /nodejs/aspose.cells/systemtimeinterruptmonitor/
---

## SystemTimeInterruptMonitor class

Simple implementation of AbstractInterruptMonitor by checking and comparing current system time with user specified limit. This implementation is just a simple solution for simple scenarios. It needs to frequently retrieve and check the system time so itself may have a negative impact on performance to some extent.

```js
new SystemTimeInterruptMonitor(terminateWithoutException)
```

Constructs one interruption monitor.

## Methods

| Name | Description |
| --- | --- |
| [getTerminateWithoutException()](#getterminatewithoutexception) | See TerminateWithoutException. This property is specified by user when constructing this monitor instance. |
| [isInterruptionRequested()](#isinterruptionrequested) | This implementation just checks whether the time cost(from the time when starting this monitor to now) is greater than u |
| [startMonitor(msLimit)](#startmonitor) | Starts the monitor with the specified time limit. The start time to calculate time cost is just when this method is call |

### getTerminateWithoutException() {#getterminatewithoutexception}

See TerminateWithoutException. This property is specified by user when constructing this monitor instance.

### isInterruptionRequested() {#isinterruptionrequested}

This implementation just checks whether the time cost(from the time when starting this monitor to now) is greater than user specified limit.

### startMonitor(msLimit) {#startmonitor}

Starts the monitor with the specified time limit. The start time to calculate time cost is just when this method is called, so the procedure which needs to be monitored should be started just after this call.

| Parameter | Type | Description |
| --- | --- | --- |
| msLimit | Number | time limit(ms) to require the interruption. |
