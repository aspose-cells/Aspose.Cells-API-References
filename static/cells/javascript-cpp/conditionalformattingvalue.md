##ConditionalFormattingValue
Describes the values of the interpolation points in a gradient scale dataBar or iconSet.
## ConditionalFormattingValue class
Describes the values of the interpolation points in a gradient scale, dataBar or iconSet.
```javascript
class ConditionalFormattingValue;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [value](#value--)| VObject | Get or set the value of this conditional formatting value object. It should be used in conjunction with Type. |
| [type](#type--)| FormatConditionValueType | Get or set the type of this conditional formatting value object. Setting the type to FormatConditionValueType.Min or FormatConditionValueType.Max will auto set "Value" to null. |
| [isGTE](#isGTE--)| boolean | Get or set the Greater Than Or Equal flag. Use only for icon sets, determines whether this threshold value uses the greater than or equal to operator. 'false' indicates 'greater than' is used instead of 'greater than or equal to'. Default value is true. |
### value {#value--}
Get or set the value of this conditional formatting value object. It should be used in conjunction with Type.
```javascript
value : VObject;
```
**Remarks**
If the value is string and start with "=", it will be processed as a formula, otherwise we will process it as a simple value.
### type {#type--}
Get or set the type of this conditional formatting value object. Setting the type to FormatConditionValueType.Min or FormatConditionValueType.Max will auto set "Value" to null.
```javascript
type : FormatConditionValueType;
```
### isGTE {#isGTE--}
Get or set the Greater Than Or Equal flag. Use only for icon sets, determines whether this threshold value uses the greater than or equal to operator. 'false' indicates 'greater than' is used instead of 'greater than or equal to'. Default value is true.
```javascript
isGTE : boolean;
```
