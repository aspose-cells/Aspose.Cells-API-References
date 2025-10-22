##IsInterruptionRequested Method
'IsInterruptionRequested method. Encapsulates the function that represents isinterruptionrequested in Go.'
## IsInterruptionRequested function
This implementation just checks whether the time cost(from the time when starting this monitor to now) is greater than user specified limit.
```go
func (instance *SystemTimeInterruptMonitor) IsInterruptionRequested()  (bool,  error)
```
## Remarks
## See Also
* Class [SystemTimeInterruptMonitor](../)
* Library [Aspose.Cells for Go](../../)
