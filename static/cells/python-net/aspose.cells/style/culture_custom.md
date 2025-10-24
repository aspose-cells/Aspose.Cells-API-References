##culture_custom property
## culture_custom property
Gets and sets the culture-dependent pattern string for number format.
If no number format has been set for this object, null will be returned.
If number format is builtin, the pattern string corresponding to the builtin number will be returned.
### Remarks
For builtin number format, both the pattern content(such as, one builtin date format is "m/d/y" for some locales,
but for some other locales it becomes  "d/m/y") and the format specifier(such as,
some locales is using character other than 'y' to represent the year part for date formatting)
are culture-dependent;
For user specified custom format, only format specifiers are changed according to the culture,
other parts of the formatting pattern will not be modified.
### Definition:
```python
@property
def culture_custom(self):
...
@culture_custom.setter
def culture_custom(self, value):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`Style`](/cells/python-net/aspose.cells/style)
