##IconSet Class
'IconSet class. Encapsulates the object that represents iconset in Go.'
## IconSet class
Describe the IconSet conditional formatting rule.This conditional formatting rule applies icons to cellsaccording to their values.
```go
type IconSet struct  {
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
|[GetCfIcons](./getcficons/) | Get theConditionalFormattingIcon from the collection |
|[GetCfvos](./getcfvos/) | Get the CFValueObjects instance. |
|[GetType](./gettype/) | Get or Set the icon set type to display.Setting the type will auto check if the current Cfvos's count isaccord with the new type. If not accord, old Cfvos will be cleaned anddefault Cfvos will be added. |
|[SetType](./settype/) | Get or Set the icon set type to display.Setting the type will auto check if the current Cfvos's count isaccord with the new type. If not accord, old Cfvos will be cleaned anddefault Cfvos will be added. |
|[IsCustom](./iscustom/) | Indicates whether the icon set is custom.Default value is false. |
|[GetShowValue](./getshowvalue/) | Get or set the flag indicating whether to show the values of the cells on which this icon set is applied.Default value is true. |
|[SetShowValue](./setshowvalue/) | Get or set the flag indicating whether to show the values of the cells on which this icon set is applied.Default value is true. |
|[GetReverse](./getreverse/) | Get or set the flag indicating whether to reverses the default order of the icons in this icon set.Default value is false. |
|[SetReverse](./setreverse/) | Get or set the flag indicating whether to reverses the default order of the icons in this icon set.Default value is false. |
