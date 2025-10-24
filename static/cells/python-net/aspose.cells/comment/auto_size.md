##auto_size property
## auto_size property
Indicates if size of comment is adjusted automatically according to its content.
Note: In some special cases (such as Mac environment), this setting may not take effect. If this setting does not take effect, please replace it with FitToTextSize().
### Example
```python
if notcomment1.auto_size:
# The size of the comment varies with the content
comment1.auto_size = True
```
### Definition:
```python
@property
def auto_size(self):
...
@auto_size.setter
def auto_size(self, value):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`Comment`](/cells/python-net/aspose.cells/comment)
