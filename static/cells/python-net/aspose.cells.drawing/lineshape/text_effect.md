##text_effect property
## text_effect property
Returns a TextEffectFormat object that contains text-effect formatting properties for the specified shape.
Applies to Shape objects that represent WordArt.
### Example
```python
if shape.is_word_art:
textEffectFormat = shape.text_effect
```
### Definition:
```python
@property
def text_effect(self):
...
```
### See Also
* module [`aspose.cells.drawing`](../../)
* class [`LineShape`](/cells/python-net/aspose.cells.drawing/lineshape)
* class [`TextEffectFormat`](/cells/python-net/aspose.cells.drawing/texteffectformat)
