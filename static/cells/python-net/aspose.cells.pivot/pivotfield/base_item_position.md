##base_item_position property
## base_item_position property
Represents the item in the base field for a custom calculation when the ShowDataAs calculation is in use.
Valid only for data fields.
Because PivotItemPosition.Custom is only for read,if you need to set PivotItemPosition.Custom,
please set PivotField.BaseItemIndex attribute.
### Remarks
NOTE: This property is now obsolete. Instead,
please use PivotField.ShowValuesSetting.BaseItemPositionType property instead.
This method will be removed 12 months later since June 2024.
Aspose apologizes for any inconvenience you may have experienced.
### Definition:
```python
@property
def base_item_position(self):
...
@base_item_position.setter
def base_item_position(self, value):
...
```
### See Also
* module [`aspose.cells.pivot`](../../)
* class [`PivotField`](/cells/python-net/aspose.cells.pivot/pivotfield)
* class [`PivotItemPosition`](/cells/python-net/aspose.cells.pivot/pivotitemposition)
