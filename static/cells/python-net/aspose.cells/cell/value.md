##value property
## value property
Gets/sets the value contained in this cell.
### Remarks
Possible type:
null,
Boolean,
DateTime,
Double,
Integer
String.
For int value, it may be returned as an Integer object or a Double object.
And there is no guarantee that the returned value will be kept as the same type of object always.
### Definition:
```python
@property
def value(self):
...
@value.setter
def value(self, value):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`Cell`](/cells/python-net/aspose.cells/cell)
