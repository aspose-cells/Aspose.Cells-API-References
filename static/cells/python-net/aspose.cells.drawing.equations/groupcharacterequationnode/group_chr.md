##group_chr property
## group_chr property
Specifies a symbol(default U+23DF).
It is strongly recommended to use attribute ChrType to set accent character.
Use this property setting if you cannot find the character you need in a known type.
### Remarks
It should be noted that this property only accepts one character, and if multiple characters are passed in, only the first character is accepted.
### Definition:
```python
@property
def group_chr(self):
...
@group_chr.setter
def group_chr(self, value):
...
```
### See Also
* module [`aspose.cells.drawing.equations`](../../)
* class [`GroupCharacterEquationNode`](/cells/python-net/aspose.cells.drawing.equations/groupcharacterequationnode)
