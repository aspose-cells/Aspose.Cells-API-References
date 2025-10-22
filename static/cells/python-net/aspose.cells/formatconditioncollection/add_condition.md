##add_condition method
## add_condition(self, type) {#aspose.cells.FormatConditionType}
Add a format condition.
### Returns
Formatting condition object index;
```python
def add_condition(self, type):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| type | aspose.cells.FormatConditionType | Format condition type. |
## add_condition(self, type, operator_type, formula1, formula2) {#aspose.cells.FormatConditionType-aspose.cells.OperatorType-System.String-System.String}
Adds a formatting condition.
### Returns
Formatting condition object index;
```python
def add_condition(self, type, operator_type, formula1, formula2):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| type | aspose.cells.FormatConditionType | The type of format condition. |
| operator_type | aspose.cells.OperatorType | The operator type |
| formula1 | System.String | The value or expression associated with conditional formatting.
| formula2 | System.String | The value or expression associated with conditional formatting.
### See Also
* module [`aspose.cells`](../../)
* class [`FormatConditionCollection`](/cells/python-net/aspose.cells/formatconditioncollection)
