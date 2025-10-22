##DefaultStyleSettings Class
'DefaultStyleSettings class. Encapsulates the object that represents defaultstylesettings in Go.'
## DefaultStyleSettings class
Settings for the default values of workbook's style properties.
```go
type DefaultStyleSettings struct  {
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
|[GetBuiltInPreference](./getbuiltinpreference/) | Indicates whether property for number format is preferable when the style defines both built-in number and custom pattern.Default value is false, that means by default custom pattern will be used to format values as long as it is not empty for one style. |
|[SetBuiltInPreference](./setbuiltinpreference/) | Indicates whether property for number format is preferable when the style defines both built-in number and custom pattern.Default value is false, that means by default custom pattern will be used to format values as long as it is not empty for one style. |
|[GetFontName](./getfontname/) | Gets/Sets the default font name for the workbook |
|[SetFontName](./setfontname/) | Gets/Sets the default font name for the workbook |
|[GetFontSize](./getfontsize/) | Gets/Sets the default standard font size for the workbook. |
|[SetFontSize](./setfontsize/) | Gets/Sets the default standard font size for the workbook. |
|[GetHorizontalAlignment](./gethorizontalalignment/) | Gets/Sets the default value for horizontal alignment |
|[SetHorizontalAlignment](./sethorizontalalignment/) | Gets/Sets the default value for horizontal alignment |
|[GetVerticalAlignment](./getverticalalignment/) | Gets/Sets the default value for vertical alignment |
|[SetVerticalAlignment](./setverticalalignment/) | Gets/Sets the default value for vertical alignment |
