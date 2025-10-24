##ThreadInterruptMonitor class
## ThreadInterruptMonitor class
Simple implementation of AbstractInterruptMonitor by starting another thread to require the interruption after sleeping user specified limit.
**Inheritance:** [`ThreadInterruptMonitor`](/cells/python-net/aspose.cells/threadinterruptmonitor)
The ThreadInterruptMonitor type exposes the following members:
### Constructors
| Constructor | Description |
| :- | :- |
| [`__init__(self, terminate_without_exception)`](/cells/python-net/aspose.cells/threadinterruptmonitor/__init__/#bool) | Constructs one interruption monitor. |
### Properties
| Property | Description |
| :- | :- |
| [is_interruption_requested](/cells/python-net/aspose.cells/threadinterruptmonitor/is_interruption_requested) | This implementation just checks whether the time cost(from the time when starting this monitor to now) is greater than user specified limit. |
| [terminate_without_exception](/cells/python-net/aspose.cells/threadinterruptmonitor/terminate_without_exception) | See TerminateWithoutException.
### Methods
| Method | Description |
| :- | :- |
| [`start_monitor(self, ms_limit)`](/cells/python-net/aspose.cells/threadinterruptmonitor/start_monitor/#int) | Starts the monitor with the specified time limit. The start time to calculate time cost is just when this method is called,
| [`finish_monitor(self)`](/cells/python-net/aspose.cells/threadinterruptmonitor/finish_monitor/#) | Finishes the monitor for one procedure. |
### Remarks
One monitor instance can be used repeatedly, as long as you monitor each process in sequence.
It should not be used to monitor multiple procedures concurrently in multi-threads.
### Example
The following example shows how to monitor the load and save procedure with specified time limit:
```python
from aspose.cells import LoadOptions, ThreadInterruptMonitor, Workbook
monitor = ThreadInterruptMonitor(False)
lopts = LoadOptions()
lopts.interrupt_monitor = monitor
monitor.start_monitor(1000)
wb = Workbook("Large.xlsx", lopts)
# if the time cost of loading the template file exceeds one second, interruption will be required and exception will be thrown here
# otherwise finishes the monitor thread and starts to monitor the save procedure
monitor.finish_monitor()
monitor.start_monitor(1500)
wb.save("result.xlsx")
monitor.finish_monitor()
```
### See Also
* module [`aspose.cells`](..)
* class [`ThreadInterruptMonitor`](/cells/python-net/aspose.cells/threadinterruptmonitor)
