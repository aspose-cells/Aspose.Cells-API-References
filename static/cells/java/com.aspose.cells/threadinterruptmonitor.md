##ThreadInterruptMonitor
Simple implementation of  by starting another thread to require the interruption after sleeping user specified limit.
**Inheritance:**
java.lang.Object, [com.aspose.cells.AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor)
```
public class ThreadInterruptMonitor extends AbstractInterruptMonitor
```
Simple implementation of [AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor) by starting another thread to require the interruption after sleeping user specified limit.
**Remarks**
One monitor instance can be used repeatedly, as long as you monitor each process in sequence. It should not be used to monitor multiple procedures concurrently in multi-threads.
**Example**
The following example shows how to monitor the load and save procedure with specified time limit:
```
ThreadInterruptMonitor monitor = new ThreadInterruptMonitor(false);
LoadOptions lopts = new LoadOptions();
lopts.setInterruptMonitor(monitor);
monitor.startMonitor(1000); //time limit is 1 second
Workbook wb = new Workbook("Large.xlsx", lopts);
//if the time cost of loading the template file exceeds one second, interruption will be required and exception will be thrown here
//otherwise finishes the monitor thread and starts to monitor the save procedure
monitor.finishMonitor();
monitor.startMonitor(1500); //time limit is 1.5 seconds
wb.save("result.xlsx");
monitor.finishMonitor();
```
## Constructors
| Constructor | Description |
| --- | --- |
| [ThreadInterruptMonitor(boolean terminateWithoutException)](#ThreadInterruptMonitor-boolean-) | Constructs one interruption monitor. |
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [finishMonitor()](#finishMonitor--) | Finishes the monitor for one procedure. |
| [getClass()](#getClass--) |  |
| [getTerminateWithoutException()](#getTerminateWithoutException--) | See [AbstractInterruptMonitor.getTerminateWithoutException()](../../com.aspose.cells/abstractinterruptmonitor\#getTerminateWithoutException--). |
| [hashCode()](#hashCode--) |  |
| [isInterruptionRequested()](#isInterruptionRequested--) | This implementation just checks whether the time cost(from the time when starting this monitor to now) is greater than user specified limit. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [startMonitor(int msLimit)](#startMonitor-int-) | Starts the monitor with the specified time limit. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ThreadInterruptMonitor(boolean terminateWithoutException) {#ThreadInterruptMonitor-boolean-}
```
public ThreadInterruptMonitor(boolean terminateWithoutException)
```
Constructs one interruption monitor.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| terminateWithoutException | boolean | [AbstractInterruptMonitor.getTerminateWithoutException()](../../com.aspose.cells/abstractinterruptmonitor\#getTerminateWithoutException--) |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |
**Returns:**
boolean
### finishMonitor() {#finishMonitor--}
```
public void finishMonitor()
```
Finishes the monitor for one procedure.
**Remarks**
Calling this method after the monitored procedure can release the monitor thread earlier, especially when there is no interruption for it(the time cost of that procedure is less than the specified time limit).
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getTerminateWithoutException() {#getTerminateWithoutException--}
```
public boolean getTerminateWithoutException()
```
See [AbstractInterruptMonitor.getTerminateWithoutException()](../../com.aspose.cells/abstractinterruptmonitor\#getTerminateWithoutException--). This property is specified by user when constructing this monitor instance.
**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### isInterruptionRequested() {#isInterruptionRequested--}
```
public boolean isInterruptionRequested()
```
This implementation just checks whether the time cost(from the time when starting this monitor to now) is greater than user specified limit.
**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```
### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```
### startMonitor(int msLimit) {#startMonitor-int-}
```
public void startMonitor(int msLimit)
```
Starts the monitor with the specified time limit. The start time to calculate time cost is just when this method is called, so the procedure which needs to be monitored should be started just after this call.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| msLimit | int | time limit(ms) to require the interruption. |
### toString() {#toString--}
```
public String toString()
```
**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```
### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |
