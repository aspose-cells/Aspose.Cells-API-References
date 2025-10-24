##GetTerminateWithoutException Method
'GetTerminateWithoutException method. Encapsulates the function that represents getterminatewithoutexception in Go.'
## GetTerminateWithoutException function
When procedure is interrupted, whether terminate the procedure quietly or throw an Exception.Default is false, that is, when IsInterruptionRequested is true,a CellsException with code ExceptionType.Interrupted will be thrown.
```go
func (instance *AbstractInterruptMonitor) GetTerminateWithoutException()  (bool,  error)
```
## Remarks
## See Also
* Class [AbstractInterruptMonitor](../)
* Library [Aspose.Cells for Go](../../)
