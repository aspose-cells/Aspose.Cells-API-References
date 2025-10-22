##value property
## value property
Get or set the value of this conditional formatting value object.
It should be used in conjunction with Type.
### Remarks
If the value is string and start with "=", it will be processed as a formula,
otherwise we will process it as a simple value.
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
* class [`ConditionalFormattingValue`](/cells/python-net/aspose.cells/conditionalformattingvalue)
