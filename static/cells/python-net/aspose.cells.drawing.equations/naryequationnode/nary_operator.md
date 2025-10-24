##nary_operator property
## nary_operator property
an n-ary operator.e.g "∑".
It is strongly recommended to use attribute NaryOperatorType to set n-ary operator.
Use this property setting if you cannot find the character you need in a known type.
### Remarks
It should be noted that this property only accepts one character, and if multiple characters are passed in, only the first character is accepted.
### Definition:
```python
@property
def nary_operator(self):
...
@nary_operator.setter
def nary_operator(self, value):
...
```
### See Also
* module [`aspose.cells.drawing.equations`](../../)
* class [`NaryEquationNode`](/cells/python-net/aspose.cells.drawing.equations/naryequationnode)
