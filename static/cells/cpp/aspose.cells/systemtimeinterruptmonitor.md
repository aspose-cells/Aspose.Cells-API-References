##Aspose::Cells::SystemTimeInterruptMonitor class
'Aspose::Cells::SystemTimeInterruptMonitor class. Simple implementation of AbstractInterruptMonitor by checking and comparing current system time with user specified limit in C++.'
## SystemTimeInterruptMonitor class
Simple implementation of [AbstractInterruptMonitor](../abstractinterruptmonitor/) by checking and comparing current system time with user specified limit.
```cpp
class SystemTimeInterruptMonitor
```
## Methods
| Method | Description |
| --- | --- |
| [GetTerminateWithoutException()](./getterminatewithoutexception/) | See AbstractInterruptMonitor.TerminateWithoutException. This property is specified by user when constructing this monitor instance. |
| [IsInterruptionRequested()](./isinterruptionrequested/) | This implementation just checks whether the time cost(from the time when starting this monitor to now) is greater than user specified limit. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const SystemTimeInterruptMonitor\& src)](./operator_asm/) | operator= |
| [StartMonitor(int32_t msLimit)](./startmonitor/) | Starts the monitor with the specified time limit. The start time to calculate time cost is just when this method is called, so the procedure which needs to be monitored should be started just after this call. |
| explicit [SystemTimeInterruptMonitor(bool terminateWithoutException)](./systemtimeinterruptmonitor/) | Constructs one interruption monitor. |
| [SystemTimeInterruptMonitor(SystemTimeInterruptMonitor_Impl* impl)](./systemtimeinterruptmonitor/) | Constructs from an implementation object. |
| [SystemTimeInterruptMonitor(const SystemTimeInterruptMonitor\& src)](./systemtimeinterruptmonitor/) | Copy constructor. |
| [~SystemTimeInterruptMonitor()](./~systemtimeinterruptmonitor/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Remarks
This implementation is just a simple solution for simple scenarios. It needs to frequently retrieve and check the system time so itself may have a negative impact on performance to some extent.
## Examples
```cpp
Aspose::Cells::Startup();
//The following example shows how to monitor the load and save procedure with specified time limit:
SystemTimeInterruptMonitor  monitor(false);
LoadOptions lopts;
lopts.SetInterruptMonitor((AbstractInterruptMonitor*)&monitor);
monitor.StartMonitor(1000); //time limit is 1 second
Workbook wb(u"Large.xlsx", lopts);
//if the time cost of loading the template file exceeds one second, interruption will be required and exception will be thrown here
//otherwise starts to monitor the save procedure
monitor.StartMonitor(1500); //time limit is 1.5 seconds
wb.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
