##InterruptMonitor Class
'InterruptMonitor class. Encapsulates the object that represents interruptmonitor in Go.'
## InterruptMonitor class
Represents all operator about the interrupt.
```go
type InterruptMonitor struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewInterruptMonitor](./newinterruptmonitor/) | Default constructor. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[IsInterruptionRequested](./isinterruptionrequested/) | Mark the monitor as requesting interruption |
|[Interrupt](./interrupt/) | Interrupt the current operator. |
