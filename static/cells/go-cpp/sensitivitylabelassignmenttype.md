##SensitivityLabelAssignmentType Enum
'SensitivityLabelAssignmentType enum. Encapsulates the object that represents sensitivitylabelassignmenttype in Go.'
## SensitivityLabelAssignmentType Enum
Represents the assignment method for the sensitivity label.
```go
type SensitivityLabelAssignmentType int32
```
## Fields
| Field | Description |
| --- | --- |
|[Standard](./standard/) | Use for any sensitivity label that was not directly applied by the user. |
|[Privileged](./privileged/) | Use for any sensitivity label that was directly applied by the user. |
