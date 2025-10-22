##accent_character property
## accent_character property
This attribute specifies the type of combining diacritical mark attached to the base of the accent function. The default accent character is U+0302.
It is strongly recommended to use attribute AccentType to set accent character.
Use this property setting if you cannot find the character you need in a known type.
### Remarks
It should be noted that this property only accepts one character, and if multiple characters are passed in, only the first character is accepted.
### Definition:
```python
@property
def accent_character(self):
...
@accent_character.setter
def accent_character(self, value):
...
```
### See Also
* module [`aspose.cells.drawing.equations`](../../)
* class [`AccentEquationNode`](/cells/python-net/aspose.cells.drawing.equations/accentequationnode)
