##load_time_out property
## load_time_out property
Sets/Gets a timeout interrupt in milliseconds in loading file, when the cost time period of loading file  is longer than the expectation   ，it will raise exception.
the default value is -1,which means no timeout interrupt is set .
### Definition:
```python
@property
def load_time_out(self):
...
@load_time_out.setter
def load_time_out(self, value):
...
```
### See Also
* module [`aspose.cellsgridjs`](../../)
* class [`Config`](/cells/python-net/aspose.cellsgridjs/config)
