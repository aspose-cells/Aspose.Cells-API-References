##VisibilityType Enum
'VisibilityType enum. Encapsulates the object that represents visibilitytype in Go.'
## VisibilityType Enum
Represents the states for sheet visibility.
```go
type VisibilityType int32
```
## Fields
| Field | Description |
| --- | --- |
|[Visible](./visible/) | Indicates the sheet is visible. |
|[Hidden](./hidden/) | Indicates the sheet is hidden, but can be shown by the user via the user interface. |
|[VeryHidden](./veryhidden/) | Indicates the sheet is hidden and cannot be shown in the user interface (UI).This state is only available programmatically. |
