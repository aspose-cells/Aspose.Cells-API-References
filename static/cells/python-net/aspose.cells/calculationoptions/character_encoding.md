##character_encoding property
## character_encoding property
Specifies the encoding used for encoding/decoding characters when calculating formulas.
For functions such as CHAR, CODE, the calculated result depends on the region settings and default charset of the environment.
With this property user can specify the proper encoding used for those function to get the expected result.
### Definition:
```python
@property
def character_encoding(self):
...
@character_encoding.setter
def character_encoding(self, value):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`CalculationOptions`](/cells/python-net/aspose.cells/calculationoptions)
