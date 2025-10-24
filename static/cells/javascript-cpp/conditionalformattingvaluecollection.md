##ConditionalFormattingValueCollection
Describes a collection of CFValueObject. Use only for icon sets.
## ConditionalFormattingValueCollection class
Describes a collection of CFValueObject. Use only for icon sets.
```javascript
class ConditionalFormattingValueCollection;
```
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Get the CFValueObject element at the specified index. |
| [add(FormatConditionValueType, string)](#add-formatconditionvaluetype-string-)| Adds [ConditionalFormattingValue](../conditionalformattingvalue/) object. |
### get(number) {#get-number-}
Get the CFValueObject element at the specified index.
```javascript
get(index: number) : ConditionalFormattingValue;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The zero based index of the element. |
**Returns**
The element at the specified index.
### add(FormatConditionValueType, string) {#add-formatconditionvaluetype-string-}
Adds [ConditionalFormattingValue](../conditionalformattingvalue/) object.
```javascript
add(type: FormatConditionValueType, value: string) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [FormatConditionValueType](../formatconditionvaluetype/) | The value type. |
| value | string | The value. |
**Returns**
Returns the index of new object in the list.
