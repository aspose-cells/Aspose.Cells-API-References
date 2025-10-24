##Aspose::Cells::AbstractInterruptMonitor class
'Aspose::Cells::AbstractInterruptMonitor class. Monitor for interruption requests in all time-consuming operations in C++.'
## AbstractInterruptMonitor class
Monitor for interruption requests in all time-consuming operations.
```cpp
class AbstractInterruptMonitor
```
## Methods
| Method | Description |
| --- | --- |
| virtual [GetTerminateWithoutException()](./getterminatewithoutexception/) | When procedure is interrupted, whether terminate the procedure quietly or throw an Exception. Default is false, that is, when [IsInterruptionRequested](./isinterruptionrequested/) is true, a [CellsException](../cellsexception/) with code [ExceptionType.Interrupted](../exceptiontype/) will be thrown. |
| virtual [IsInterruptionRequested()](./isinterruptionrequested/) | Indicates whether interruption is requested for current operation. If true then current operation will be interrupted. Implementation should perform fast and efficient check here, otherwise it may become another bottleneck for the procedure. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
