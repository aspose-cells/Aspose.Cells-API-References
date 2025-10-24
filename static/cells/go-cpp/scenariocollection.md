##ScenarioCollection Class
'ScenarioCollection class. Encapsulates the object that represents scenariocollection in Go.'
## ScenarioCollection class
Represents the list of scenarios.
```go
type ScenarioCollection struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetActiveIndex](./getactiveindex/) | Gets and sets which scenario is selected. |
|[SetActiveIndex](./setactiveindex/) | Gets and sets which scenario is selected. |
|[GetLastSelected](./getlastselected/) | Indicates which scenario was last selected by the user to be run/shown. |
|[SetLastSelected](./setlastselected/) | Indicates which scenario was last selected by the user to be run/shown. |
|[Get](./get/) | Gets the Scenario object by the index. |
|[Add](./add/) | Adds a scenario. |
|[GetCount](./getcount/) |  |
