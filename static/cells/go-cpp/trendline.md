##Trendline Class
'Trendline class. Encapsulates the object that represents trendline in Go.'
## Trendline class
Represents a trendline in a chart.
```go
type Trendline struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewTrendline](./newtrendline/) | Constructs from a parent object. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[IsNameAuto](./isnameauto/) | Returns if Microsoft Excel automatically determines the name of the trendline. |
|[SetIsNameAuto](./setisnameauto/) | Returns if Microsoft Excel automatically determines the name of the trendline. |
|[GetType](./gettype/) | Returns the trendline type. |
|[GetName](./getname/) | Returns the name of the trendline. |
|[SetName](./setname/) | Returns the name of the trendline. |
|[GetOrder](./getorder/) | Returns or sets the trendline order (an integer greater than 1) when the trendline type is Polynomial.The order must be between 2 and 6. |
|[SetOrder](./setorder/) | Returns or sets the trendline order (an integer greater than 1) when the trendline type is Polynomial.The order must be between 2 and 6. |
|[GetPeriod](./getperiod/) | Returns or sets the period for the moving-average trendline. |
|[SetPeriod](./setperiod/) | Returns or sets the period for the moving-average trendline. |
|[GetForward](./getforward/) | Returns or sets the number of periods (or units on a scatter chart) that the trendline extends forward.The number of periods must be greater than or equal to zero. |
|[SetForward](./setforward/) | Returns or sets the number of periods (or units on a scatter chart) that the trendline extends forward.The number of periods must be greater than or equal to zero. |
|[GetBackward](./getbackward/) | Returns or sets the number of periods (or units on a scatter chart) that the trendline extends backward.The number of periods must be greater than or equal to zero.If the chart type is column ,the number of periods must be between 0 and 0.5 |
|[SetBackward](./setbackward/) | Returns or sets the number of periods (or units on a scatter chart) that the trendline extends backward.The number of periods must be greater than or equal to zero.If the chart type is column ,the number of periods must be between 0 and 0.5 |
|[GetDisplayEquation](./getdisplayequation/) | Represents if the equation for the trendline is displayed on the chart (in the same data label as the R-squared value). Setting this property to True automatically turns on data labels. |
|[SetDisplayEquation](./setdisplayequation/) | Represents if the equation for the trendline is displayed on the chart (in the same data label as the R-squared value). Setting this property to True automatically turns on data labels. |
|[GetDisplayRSquared](./getdisplayrsquared/) | Represents if the R-squared value of the trendline is displayed on the chart (in the same data label as the equation). Setting this property to True automatically turns on data labels. |
|[SetDisplayRSquared](./setdisplayrsquared/) | Represents if the R-squared value of the trendline is displayed on the chart (in the same data label as the equation). Setting this property to True automatically turns on data labels. |
|[GetIntercept](./getintercept/) | Returns or sets the point where the trendline crosses the value axis. |
|[SetIntercept](./setintercept/) | Returns or sets the point where the trendline crosses the value axis. |
|[GetDataLabels](./getdatalabels/) | Represents the DataLabels object for the specified series. |
|[GetLegendEntry](./getlegendentry/) | Gets the legend entry according to this trendline |
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
