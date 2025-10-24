##std_dev property
## std_dev property
Get or set the number of standard deviations to include above or below the average in the
conditional formatting rule.
The input value must between 0 and 3 (include 0 and 3).
Setting this value to 0 means stdDev is not set.
The default value is 0.
### Definition:
```python
@property
def std_dev(self):
...
@std_dev.setter
def std_dev(self, value):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`AboveAverage`](/cells/python-net/aspose.cells/aboveaverage)
