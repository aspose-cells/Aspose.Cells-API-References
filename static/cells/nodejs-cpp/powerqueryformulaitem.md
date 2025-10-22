##PowerQueryFormulaItem
Represents the item of the power query formula.
## PowerQueryFormulaItem class
Represents the item of the power query formula.
```javascript
class PowerQueryFormulaItem;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [name](#name--)| string | Readonly. Gets the name of the item. |
| [value](#value--)| string | Gets the value of the item. |
## Methods
| Method | Description |
| --- | --- |
| [getName()](#getName--)| <b>@deprecated.</b> Please use the 'name' property instead. Gets the name of the item. |
| [getValue()](#getValue--)| <b>@deprecated.</b> Please use the 'value' property instead. Gets the value of the item. |
| [setValue(string)](#setValue-string-)| <b>@deprecated.</b> Please use the 'value' property instead. Gets the value of the item. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### name {#name--}
Readonly. Gets the name of the item.
```javascript
name : string;
```
### value {#value--}
Gets the value of the item.
```javascript
value : string;
```
### getName() {#getName--}
```javascript
getName() : string;
```
### getValue() {#getValue--}
```javascript
getValue() : string;
```
### setValue(string) {#setValue-string-}
```javascript
setValue(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
