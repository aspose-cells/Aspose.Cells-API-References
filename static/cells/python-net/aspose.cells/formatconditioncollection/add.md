##add method
## add(self, cell_area, type, operator_type, formula1, formula2) {#aspose.cells.CellArea-aspose.cells.FormatConditionType-aspose.cells.OperatorType-System.String-System.String}
Adds a formatting condition and effected cell rang to the FormatConditions
The FormatConditions can contain up to three conditional formats.
References to the other sheets are not allowed in the formulas of conditional formatting.
### Returns
[0]:Formatting condition object index;[1] Effected cell rang index.
```python
def add(self, cell_area, type, operator_type, formula1, formula2):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| cell_area | aspose.cells.CellArea | Conditional formatted cell range. |
| type | aspose.cells.FormatConditionType | Type of conditional formatting.It could be one of the members of FormatConditionType. |
| operator_type | aspose.cells.OperatorType | Comparison operator.It could be one of the members of OperatorType. |
| formula1 | System.String | The value or expression associated with conditional formatting. |
| formula2 | System.String | The value or expression associated with conditional formatting |
### See Also
* module [`aspose.cells`](../../)
* class [`FormatConditionCollection`](/cells/python-net/aspose.cells/formatconditioncollection)
