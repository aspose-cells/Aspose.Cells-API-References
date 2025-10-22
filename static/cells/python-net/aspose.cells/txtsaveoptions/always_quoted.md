##always_quoted property
## always_quoted property
Indicates whether always adding '"' for each field.
If true then all values will be quoted;
If false then values will only be quoted when needed(for example,
when values contain special characters such as '"' , '\n' or separator character).
Default is false.
### Remarks
NOTE: This member is now obsolete. Instead,
please use QuoteType property instead.
This property will be removed 12 months later since August 2012.
Aspose apologizes for any inconvenience you may have experienced.
### Definition:
```python
@property
def always_quoted(self):
...
@always_quoted.setter
def always_quoted(self, value):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`TxtSaveOptions`](/cells/python-net/aspose.cells/txtsaveoptions)
