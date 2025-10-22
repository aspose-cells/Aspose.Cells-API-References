##WebExtensionProperty
Represents an Office Addin custom property.
## WebExtensionProperty class
Represents an Office Add-in custom property.
```javascript
class WebExtensionProperty;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [name](#name--)| string | Gets and set a custom property name. |
| [value](#value--)| string | Gets and sets a custom property value. |
## Methods
| Method | Description |
| --- | --- |
| [getName()](#getName--)| <b>@deprecated.</b> Please use the 'name' property instead. Gets and set a custom property name. |
| [setName(string)](#setName-string-)| <b>@deprecated.</b> Please use the 'name' property instead. Gets and set a custom property name. |
| [getValue()](#getValue--)| <b>@deprecated.</b> Please use the 'value' property instead. Gets and sets a custom property value. |
| [setValue(string)](#setValue-string-)| <b>@deprecated.</b> Please use the 'value' property instead. Gets and sets a custom property value. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### name {#name--}
Gets and set a custom property name.
```javascript
name : string;
```
### value {#value--}
Gets and sets a custom property value.
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
