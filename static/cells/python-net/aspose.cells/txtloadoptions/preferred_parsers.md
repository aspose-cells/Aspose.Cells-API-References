##preferred_parsers property
## preferred_parsers property
Gets and sets preferred value parsers for loading text file.
### Remarks
parsers[0] is the parser will be used for the first column in text template file,
parsers[1] is the parser will be used for the second column, ...etc.
The last one(parsers[parsers.length-1]) will be used for all other columns start from parsers.length-1.
If one item is null, the corresponding column will be parsed by the default parser of Aspose.Cells.
### Definition:
```python
@property
def preferred_parsers(self):
...
@preferred_parsers.setter
def preferred_parsers(self, value):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`TxtLoadOptions`](/cells/python-net/aspose.cells/txtloadoptions)
