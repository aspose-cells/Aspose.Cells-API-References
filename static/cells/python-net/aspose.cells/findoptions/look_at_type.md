##look_at_type property
## look_at_type property
Look at type.
### Remarks
When [`FindOptions.regex_key`](/cells/python-net/aspose.cells/findoptions#regex_key) is true and user has specified the exact rule for the regex,
for performance consideration this property should be set as [`LookAtType.ENTIRE_CONTENT`](/cells/python-net/aspose.cells/lookattype#ENTIRE_CONTENT).
Otherwise we will refactor the search key to ensure it can be matched according to the specific type.
For example, when the type is [`LookAtType.CONTAINS`](/cells/python-net/aspose.cells/lookattype#CONTAINS)(this is the default value for this property),
we will add wildcards at the beginning and end of the search key automatically.
In this case, the regular expressions will become more complex and the performance will also decrease.
### Definition:
```python
@property
def look_at_type(self):
...
@look_at_type.setter
def look_at_type(self, value):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`FindOptions`](/cells/python-net/aspose.cells/findoptions)
* class [`LookAtType`](/cells/python-net/aspose.cells/lookattype)
