##FormatCondition Class
'FormatCondition class. Encapsulates the object that represents formatcondition in Go.'
## FormatCondition class
Represents conditional formatting condition.
```go
type FormatCondition struct  {
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
|[GetFormula1_Bool_Bool](./getformula1_bool_bool/) | Gets the value or expression associated with this format condition. |
|[GetFormula2_Bool_Bool](./getformula2_bool_bool/) | Gets the value or expression associated with this format condition. |
|[GetFormula1_Bool_Bool_Int_Int](./getformula1_bool_bool_int_int/) | Gets the value or expression of the conditional formatting of the cell. |
|[GetFormula2_Bool_Bool_Int_Int](./getformula2_bool_bool_int_int/) | Gets the value or expression of the conditional formatting of the cell. |
|[SetFormulas](./setformulas/) | Sets the value or expression associated with this format condition. |
|[SetFormula1_String_Bool_Bool](./setformula1_string_bool_bool/) | Sets the value or expression associated with this format condition. |
|[SetFormula2_String_Bool_Bool](./setformula2_string_bool_bool/) | Sets the value or expression associated with this format condition. |
|[GetFormula1](./getformula1/) | Gets and sets the value or expression associated with conditional formatting. |
|[SetFormula1_String](./setformula1_string/) | Gets and sets the value or expression associated with conditional formatting. |
|[GetFormula1_Int_Int](./getformula1_int_int/) | Gets the formula of the conditional formatting of the cell. |
|[GetFormula2](./getformula2/) | Gets and sets the value or expression associated with conditional formatting. |
|[SetFormula2_String](./setformula2_string/) | Gets and sets the value or expression associated with conditional formatting. |
|[GetFormula2_Int_Int](./getformula2_int_int/) | Gets the formula of the conditional formatting of the cell. |
|[GetOperator](./getoperator/) | Gets and sets the conditional format operator type. |
|[SetOperator](./setoperator/) | Gets and sets the conditional format operator type. |
|[GetStopIfTrue](./getstopiftrue/) | True, no rules with lower priority may be applied over this rule, when this rule evaluates to true.Only applies for Excel 2007; |
|[SetStopIfTrue](./setstopiftrue/) | True, no rules with lower priority may be applied over this rule, when this rule evaluates to true.Only applies for Excel 2007; |
|[GetPriority](./getpriority/) | The priority of this conditional formatting rule. This value is used to determine whichformat should be evaluated and rendered. Lower numeric values are higher priority thanhigher numeric values, where '1' is the highest priority. |
|[SetPriority](./setpriority/) | The priority of this conditional formatting rule. This value is used to determine whichformat should be evaluated and rendered. Lower numeric values are higher priority thanhigher numeric values, where '1' is the highest priority. |
|[GetStyle](./getstyle/) | Gets or setts style of conditional formatted cell ranges. |
|[SetStyle](./setstyle/) | Gets or setts style of conditional formatted cell ranges. |
|[GetType](./gettype/) | Gets and sets whether the conditional format Type. |
|[SetType](./settype/) | Gets and sets whether the conditional format Type. |
|[GetIconSet](./geticonset/) | Get the conditional formatting's "IconSet" instance.The default instance's IconSetType is TrafficLights31.Valid only for type = IconSet. |
|[GetDataBar](./getdatabar/) | Get the conditional formatting's "DataBar" instance.The default instance's color is blue.Valid only for type is DataBar. |
|[GetColorScale](./getcolorscale/) | Get the conditional formatting's "ColorScale" instance.The default instance is a "green-yellow-red" 3ColorScale .Valid only for type = ColorScale. |
|[GetTop10](./gettop10/) | Get the conditional formatting's "Top10" instance.The default instance's rule highlights cells whosevalues fall in the top 10 bracket.Valid only for type is Top10. |
|[GetAboveAverage](./getaboveaverage/) | Get the conditional formatting's "AboveAverage" instance.The default instance's rule highlights cells that areabove the average for all values in the range.Valid only for type = AboveAverage. |
|[GetText](./gettext/) | The text value in a "text contains" conditional formatting rule.Valid only for type = containsText, notContainsText, beginsWith and endsWith.The default value is null. |
|[SetText](./settext/) | The text value in a "text contains" conditional formatting rule.Valid only for type = containsText, notContainsText, beginsWith and endsWith.The default value is null. |
|[GetTimePeriod](./gettimeperiod/) | The applicable time period in a "date occurring…" conditional formatting rule.Valid only for type = timePeriod.The default value is TimePeriodType.Today. |
|[SetTimePeriod](./settimeperiod/) | The applicable time period in a "date occurring…" conditional formatting rule.Valid only for type = timePeriod.The default value is TimePeriodType.Today. |
