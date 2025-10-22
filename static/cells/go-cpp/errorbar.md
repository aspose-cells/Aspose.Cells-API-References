##ErrorBar Class
'ErrorBar class. Encapsulates the object that represents errorbar in Go.'
## ErrorBar class
Represents error bar of data series.
```go
type ErrorBar struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewErrorBar](./newerrorbar/) | Constructs from a parent object. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetType](./gettype/) | Represents error bar amount type. |
|[SetType](./settype/) | Represents error bar amount type. |
|[GetDisplayType](./getdisplaytype/) | Represents the display type of error bar. |
|[SetDisplayType](./setdisplaytype/) | Represents the display type of error bar. |
|[GetAmount](./getamount/) | Represents amount of error bar. |
|[SetAmount](./setamount/) | Represents amount of error bar. |
|[GetShowMarkerTTop](./getshowmarkerttop/) | Indicates if formatting error bars with a T-top. |
|[SetShowMarkerTTop](./setshowmarkerttop/) | Indicates if formatting error bars with a T-top. |
|[GetPlusValue](./getplusvalue/) | Represents positive error amount when error bar type is Custom. |
|[SetPlusValue](./setplusvalue/) | Represents positive error amount when error bar type is Custom. |
|[GetMinusValue](./getminusvalue/) | Represents negative error amount when error bar type is Custom. |
|[SetMinusValue](./setminusvalue/) | Represents negative error amount when error bar type is Custom. |
|[GetCompoundType](./getcompoundtype/) | Specifies the compound line type |
|[SetCompoundType](./setcompoundtype/) | Specifies the compound line type |
|[GetDashType](./getdashtype/) | Specifies the dash line type |
|[SetDashType](./setdashtype/) | Specifies the dash line type |
|[GetCapType](./getcaptype/) | Specifies the ending caps. |
|[SetCapType](./setcaptype/) | Specifies the ending caps. |
|[GetJoinType](./getjointype/) | Specifies the joining caps. |
|[SetJoinType](./setjointype/) | Specifies the joining caps. |
|[GetBeginType](./getbegintype/) | Specifies an arrowhead for the begin of a line. |
|[SetBeginType](./setbegintype/) | Specifies an arrowhead for the begin of a line. |
|[GetEndType](./getendtype/) | Specifies an arrowhead for the end of a line. |
|[SetEndType](./setendtype/) | Specifies an arrowhead for the end of a line. |
|[GetBeginArrowLength](./getbeginarrowlength/) | Specifies the length of the arrowhead for the begin of a line. |
|[SetBeginArrowLength](./setbeginarrowlength/) | Specifies the length of the arrowhead for the begin of a line. |
|[GetEndArrowLength](./getendarrowlength/) | Specifies the length of the arrowhead for the end of a line. |
|[SetEndArrowLength](./setendarrowlength/) | Specifies the length of the arrowhead for the end of a line. |
|[GetBeginArrowWidth](./getbeginarrowwidth/) | Specifies the width of the arrowhead for the begin of a line. |
|[SetBeginArrowWidth](./setbeginarrowwidth/) | Specifies the width of the arrowhead for the begin of a line. |
|[GetEndArrowWidth](./getendarrowwidth/) | Specifies the width of the arrowhead for the end of a line. |
|[SetEndArrowWidth](./setendarrowwidth/) | Specifies the width of the arrowhead for the end of a line. |
|[GetThemeColor](./getthemecolor/) | Gets and sets the theme color. |
|[SetThemeColor](./setthemecolor/) | Gets and sets the theme color. |
|[GetColor](./getcolor/) | Represents the Color of the line. |
|[SetColor](./setcolor/) | Represents the Color of the line. |
|[GetTransparency](./gettransparency/) | Returns or sets the degree of transparency of the line as a value from 0.0 (opaque) through 1.0 (clear). |
|[SetTransparency](./settransparency/) | Returns or sets the degree of transparency of the line as a value from 0.0 (opaque) through 1.0 (clear). |
|[GetStyle](./getstyle/) | Represents the style of the line. |
|[SetStyle](./setstyle/) | Represents the style of the line. |
|[GetWeight](./getweight/) | Gets or sets the WeightType of the line. |
|[SetWeight](./setweight/) | Gets or sets the WeightType of the line. |
|[GetWeightPt](./getweightpt/) | Gets or sets the weight of the line in unit of points. |
|[SetWeightPt](./setweightpt/) | Gets or sets the weight of the line in unit of points. |
|[GetWeightPx](./getweightpx/) | Gets or sets the weight of the line in unit of pixels. |
|[SetWeightPx](./setweightpx/) | Gets or sets the weight of the line in unit of pixels. |
|[GetFormattingType](./getformattingtype/) | Gets or sets format type. |
|[SetFormattingType](./setformattingtype/) | Gets or sets format type. |
|[IsAutomaticColor](./isautomaticcolor/) | Indicates whether the color of line is automatic assigned. |
|[IsVisible](./isvisible/) | Represents whether the line is visible. |
|[SetIsVisible](./setisvisible/) | Represents whether the line is visible. |
|[IsAuto](./isauto/) | Indicates whether this line style is auto assigned. |
|[SetIsAuto](./setisauto/) | Indicates whether this line style is auto assigned. |
|[GetGradientFill](./getgradientfill/) | Represents gradient fill. |
