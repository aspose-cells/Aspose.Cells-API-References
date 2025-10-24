##base_item_position_type property
## base_item_position_type property
Represents type of the base pivot item in the base field when the ShowDataAs calculation is in use.
Valid only for data fields.
Because PivotItemPosition.Custom is only for read,if you need to set PivotItemPosition.Custom,
please set PivotField.BaseItemIndex attribute.
### Definition:
```python
@property
def base_item_position_type(self):
...
@base_item_position_type.setter
def base_item_position_type(self, value):
...
```
### See Also
* module [`aspose.cells.pivot`](../../)
* class [`PivotItemPositionType`](/cells/python-net/aspose.cells.pivot/pivotitempositiontype)
* class [`PivotShowValuesSetting`](/cells/python-net/aspose.cells.pivot/pivotshowvaluessetting)
