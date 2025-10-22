##built_in_preference property
## built_in_preference property
Indicates whether property for number format is preferable when the style defines both built-in number and custom pattern.
Default value is false, that means by default custom pattern will be used to format values as long as it is not empty for one style.
### Remarks
When loading workbook from existing template file, maybe both built-in number and custom pattern are defined for one style.
This property determine whether we should use the built-in number or the custom pattern when formatting values with the style.
### Definition:
```python
@property
def built_in_preference(self):
...
@built_in_preference.setter
def built_in_preference(self, value):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`DefaultStyleSettings`](/cells/python-net/aspose.cells/defaultstylesettings)
