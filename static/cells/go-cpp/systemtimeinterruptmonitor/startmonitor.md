##StartMonitor Method
'StartMonitor method. Encapsulates the function that represents startmonitor in Go.'
## StartMonitor function
Starts the monitor with the specified time limit. The start time to calculate time cost is just when this method is called,so the procedure which needs to be monitored should be started just after this call.
```go
func (instance *SystemTimeInterruptMonitor) StartMonitor(mslimit int32)  error
```
## Remarks
## See Also
* Class [SystemTimeInterruptMonitor](../)
* Library [Aspose.Cells for Go](../../)
