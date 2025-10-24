##AbstractInterruptMonitor Class
'AbstractInterruptMonitor class. Encapsulates the object that represents abstractinterruptmonitor in Go.'
## AbstractInterruptMonitor class
Monitor for interruption requests in all time-consuming operations.
```go
type AbstractInterruptMonitor struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
## Methods
| Method | Description |
| --- | --- |
|[GetTerminateWithoutException](./getterminatewithoutexception/) | When procedure is interrupted, whether terminate the procedure quietly or throw an Exception.Default is false, that is, when IsInterruptionRequested is true,a CellsException with code ExceptionType.Interrupted will be thrown. |
