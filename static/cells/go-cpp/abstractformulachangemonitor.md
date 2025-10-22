##AbstractFormulaChangeMonitor Class
'AbstractFormulaChangeMonitor class. Encapsulates the object that represents abstractformulachangemonitor in Go.'
## AbstractFormulaChangeMonitor class
Monitor for user to track the change of formulas during certain operations.
```go
type AbstractFormulaChangeMonitor struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
## Methods
| Method | Description |
| --- | --- |
|[OnCellFormulaChanged](./oncellformulachanged/) | The event that will be triggered when the formula in a cell is changed. |
|[OnFormatConditionFormulaChanged](./onformatconditionformulachanged/) | The event that will be triggered when the formula of FormatCondition is changed. |
