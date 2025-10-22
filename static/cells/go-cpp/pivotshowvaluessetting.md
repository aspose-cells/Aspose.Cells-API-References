##PivotShowValuesSetting Class
'PivotShowValuesSetting class. Encapsulates the object that represents pivotshowvaluessetting in Go.'
## PivotShowValuesSetting class
Represents the settings about showing values as when the ShowDataAs calculation is in use.
```go
type PivotShowValuesSetting struct  {
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
|[GetCalculationType](./getcalculationtype/) | Represents how to show values of a data field in the pivot report. |
|[SetCalculationType](./setcalculationtype/) | Represents how to show values of a data field in the pivot report. |
|[GetBaseFieldIndex](./getbasefieldindex/) | Represents the base field for a ShowDataAs calculation when the ShowDataAs calculation is in use. |
|[SetBaseFieldIndex](./setbasefieldindex/) | Represents the base field for a ShowDataAs calculation when the ShowDataAs calculation is in use. |
|[GetBaseItemPositionType](./getbaseitempositiontype/) | Represents type of the base pivot item in the base field when the ShowDataAs calculation is in use.Valid only for data fields.Because PivotItemPosition.Custom is only for read,if you need to set PivotItemPosition.Custom,please set PivotField.BaseItemIndex attribute. |
|[SetBaseItemPositionType](./setbaseitempositiontype/) | Represents type of the base pivot item in the base field when the ShowDataAs calculation is in use.Valid only for data fields.Because PivotItemPosition.Custom is only for read,if you need to set PivotItemPosition.Custom,please set PivotField.BaseItemIndex attribute. |
|[GetBaseItemIndex](./getbaseitemindex/) | Represents the custom index of the pivot item in the base field when the ShowDataAs calculation is in use.Valid only for data fields. |
|[SetBaseItemIndex](./setbaseitemindex/) | Represents the custom index of the pivot item in the base field when the ShowDataAs calculation is in use.Valid only for data fields. |
