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
| [value](#value--)| Object | Get or set the value of this conditional formatting value object. It should be used in conjunction with Type. |
| [type](#type--)| FormatConditionValueType | Get or set the type of this conditional formatting value object. Setting the type to FormatConditionValueType.Min or FormatConditionValueType.Max will auto set "Value" to null. |
| [isGTE](#isGTE--)| boolean | Get or set the Greater Than Or Equal flag. Use only for icon sets, determines whether this threshold value uses the greater than or equal to operator. 'false' indicates 'greater than' is used instead of 'greater than or equal to'. Default value is true. |
## Methods
| Method | Description |
| --- | --- |
| [getValue()](#getValue--)| <b>@deprecated.</b> Please use the 'value' property instead. Get or set the value of this conditional formatting value object. It should be used in conjunction with Type. |
| [setValue(Object)](#setValue-object-)| <b>@deprecated.</b> Please use the 'value' property instead. Get or set the value of this conditional formatting value object. It should be used in conjunction with Type. |
| [getType()](#getType--)| <b>@deprecated.</b> Please use the 'type' property instead. Get or set the type of this conditional formatting value object. Setting the type to FormatConditionValueType.Min or FormatConditionValueType.Max will auto set "Value" to null. |
| [setType(FormatConditionValueType)](#setType-formatconditionvaluetype-)| <b>@deprecated.</b> Please use the 'type' property instead. Get or set the type of this conditional formatting value object. Setting the type to FormatConditionValueType.Min or FormatConditionValueType.Max will auto set "Value" to null. |
| [isGTE()](#isGTE--)| <b>@deprecated.</b> Please use the 'isGTE' property instead. Get or set the Greater Than Or Equal flag. Use only for icon sets, determines whether this threshold value uses the greater than or equal to operator. 'false' indicates 'greater than' is used instead of 'greater than or equal to'. Default value is true. |
| [setIsGTE(boolean)](#setIsGTE-boolean-)| <b>@deprecated.</b> Please use the 'isGTE' property instead. Get or set the Greater Than Or Equal flag. Use only for icon sets, determines whether this threshold value uses the greater than or equal to operator. 'false' indicates 'greater than' is used instead of 'greater than or equal to'. Default value is true. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### value {#value--}
Get or set the value of this conditional formatting value object. It should be used in conjunction with Type.
```javascript
value : Object;
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
### getValue() {#getValue--}
```javascript
getValue() : Object;
```
**Remarks**
If the value is string and start with "=", it will be processed as a formula, otherwise we will process it as a simple value.
### setValue(Object) {#setValue-object-}
```javascript
setValue(value: Object) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | Object | The value to set. |
**Remarks**
If the value is string and start with "=", it will be processed as a formula, otherwise we will process it as a simple value.
### getType() {#getType--}
```javascript
getType() : FormatConditionValueType;
```
**Returns**
[FormatConditionValueType](../formatconditionvaluetype/)
### setType(FormatConditionValueType) {#setType-formatconditionvaluetype-}
```javascript
setType(value: FormatConditionValueType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [FormatConditionValueType](../formatconditionvaluetype/) | The value to set. |
### isGTE() {#isGTE--}
```javascript
isGTE() : boolean;
```
### setIsGTE(boolean) {#setIsGTE-boolean-}
```javascript
setIsGTE(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
