##ignore_useless_shapes property
## ignore_useless_shapes property
Indicates whether ignoring useless shapes.
### Remarks
Only works for xlsx,xlsb, and xlsm files.
There are many overlapping identical shapes which are useless in some files,
we can ingore them when loading files.
### Definition:
```python
@property
def ignore_useless_shapes(self):
...
@ignore_useless_shapes.setter
def ignore_useless_shapes(self, value):
...
```
### See Also
* module [`aspose.cells.numbers`](../../)
* class [`NumbersLoadOptions`](/cells/python-net/aspose.cells.numbers/numbersloadoptions)
