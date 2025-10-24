##VbaModule
Represents the module in VBA project.
## VbaModule class
Represents the module in VBA project.
```javascript
class VbaModule;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [name](#name--)| string | Gets and sets the name of Module. |
| [type](#type--)| VbaModuleType | Readonly. Gets the type of module. |
| [binaryCodes](#binaryCodes--)| Uint8Array | Readonly. Gets and sets the binary codes of module. |
| [codes](#codes--)| string | Gets and sets the codes of module. |
## Methods
| Method | Description |
| --- | --- |
| [getName()](#getName--)| <b>@deprecated.</b> Please use the 'name' property instead. Gets and sets the name of Module. |
| [setName(string)](#setName-string-)| <b>@deprecated.</b> Please use the 'name' property instead. Gets and sets the name of Module. |
| [getType()](#getType--)| <b>@deprecated.</b> Please use the 'type' property instead. Gets the type of module. |
| [getBinaryCodes()](#getBinaryCodes--)| <b>@deprecated.</b> Please use the 'binaryCodes' property instead. Gets and sets the binary codes of module. |
| [getCodes()](#getCodes--)| <b>@deprecated.</b> Please use the 'codes' property instead. Gets and sets the codes of module. |
| [setCodes(string)](#setCodes-string-)| <b>@deprecated.</b> Please use the 'codes' property instead. Gets and sets the codes of module. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### name {#name--}
Gets and sets the name of Module.
```javascript
name : string;
```
### type {#type--}
Readonly. Gets the type of module.
```javascript
type : VbaModuleType;
```
### binaryCodes {#binaryCodes--}
Readonly. Gets and sets the binary codes of module.
```javascript
binaryCodes : Uint8Array;
```
### codes {#codes--}
Gets and sets the codes of module.
```javascript
codes : string;
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
### getType() {#getType--}
```javascript
getType() : VbaModuleType;
```
**Returns**
[VbaModuleType](../vbamoduletype/)
### getBinaryCodes() {#getBinaryCodes--}
```javascript
getBinaryCodes() : Uint8Array;
```
### getCodes() {#getCodes--}
```javascript
getCodes() : string;
```
### setCodes(string) {#setCodes-string-}
```javascript
setCodes(value: string) : void;
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
