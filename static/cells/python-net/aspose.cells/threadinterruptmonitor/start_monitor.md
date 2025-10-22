##start_monitor method
## start_monitor(self, ms_limit) {#int}
Starts the monitor with the specified time limit. The start time to calculate time cost is just when this method is called,
so the procedure which needs to be monitored should be started just after this call.
```python
def start_monitor(self, ms_limit):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| ms_limit | int | time limit(ms) to require the interruption. |
### See Also
* module [`aspose.cells`](../../)
* class [`ThreadInterruptMonitor`](/cells/python-net/aspose.cells/threadinterruptmonitor)
