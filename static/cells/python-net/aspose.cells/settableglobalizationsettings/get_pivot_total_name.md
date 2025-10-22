##get_pivot_total_name method
## get_pivot_total_name(self) {#}
Gets the name of "Total" label in the PivotTable.
You need to override this method when the PivotTable contains two or more PivotFields in the data area.
### Returns
The name of "Total" label
```python
def get_pivot_total_name(self):
...
```
### Remarks
NOTE: This member is now obsolete. Instead,
please use PivotGlobalizationSettings.GetColumnLabelsOfPivotTable() method.
This property will be removed 12 months later since December 2022.
Aspose apologizes for any inconvenience you may have experienced.
### See Also
* module [`aspose.cells`](../../)
* class [`SettableGlobalizationSettings`](/cells/python-net/aspose.cells/settableglobalizationsettings)
