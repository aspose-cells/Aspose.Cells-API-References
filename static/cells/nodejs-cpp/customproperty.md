##CustomProperty
Represents identifier information.
## CustomProperty class
Represents identifier information.
```javascript
class CustomProperty;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [name](#name--)| string | Returns or sets the name of the object. |
| [value](#value--)| string | Returns or sets the value of the custom property. |
## Methods
| Method | Description |
| --- | --- |
| [getName()](#getName--)| <b>@deprecated.</b> Please use the 'name' property instead. Returns or sets the name of the object. |
| [setName(string)](#setName-string-)| <b>@deprecated.</b> Please use the 'name' property instead. Returns or sets the name of the object. |
| [getValue()](#getValue--)| <b>@deprecated.</b> Please use the 'value' property instead. Returns or sets the value of the custom property. |
| [setValue(string)](#setValue-string-)| <b>@deprecated.</b> Please use the 'value' property instead. Returns or sets the value of the custom property. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### constructor() {#constructor--}
Default Constructor.
```javascript
constructor();
```
### name {#name--}
Returns or sets the name of the object.
```javascript
name : string;
```
### value {#value--}
Returns or sets the value of the custom property.
```javascript
value : string;
```
### getName() {#getName--}
```javascript
getName() : string;
```
### setName(string) {#setName-string-}
```javascript
setName(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
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
