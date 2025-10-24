##WebExtensionBinding
Represents a binding relationship between an Office Addin and the data in the document.
## WebExtensionBinding class
Represents a binding relationship between an Office Add-in and the data in the document.
```javascript
class WebExtensionBinding;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [id](#id--)| string | Gets and sets the binding identifier. |
| [type](#type--)| string | Gets and sets the binding type. |
| [appref](#appref--)| string | Gets and sets the binding key used to map the binding entry in this list with the bound data in the document. |
## Methods
| Method | Description |
| --- | --- |
| [getId()](#getId--)| <b>@deprecated.</b> Please use the 'id' property instead. Gets and sets the binding identifier. |
| [setId(string)](#setId-string-)| <b>@deprecated.</b> Please use the 'id' property instead. Gets and sets the binding identifier. |
| [getType()](#getType--)| <b>@deprecated.</b> Please use the 'type' property instead. Gets and sets the binding type. |
| [setType(string)](#setType-string-)| <b>@deprecated.</b> Please use the 'type' property instead. Gets and sets the binding type. |
| [getAppref()](#getAppref--)| <b>@deprecated.</b> Please use the 'appref' property instead. Gets and sets the binding key used to map the binding entry in this list with the bound data in the document. |
| [setAppref(string)](#setAppref-string-)| <b>@deprecated.</b> Please use the 'appref' property instead. Gets and sets the binding key used to map the binding entry in this list with the bound data in the document. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### constructor() {#constructor--}
Default Constructor.
```javascript
constructor();
```
### id {#id--}
Gets and sets the binding identifier.
```javascript
id : string;
```
### type {#type--}
Gets and sets the binding type.
```javascript
type : string;
```
### appref {#appref--}
Gets and sets the binding key used to map the binding entry in this list with the bound data in the document.
```javascript
appref : string;
```
### getId() {#getId--}
```javascript
getId() : string;
```
### setId(string) {#setId-string-}
```javascript
setId(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getType() {#getType--}
```javascript
getType() : string;
```
### setType(string) {#setType-string-}
```javascript
setType(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getAppref() {#getAppref--}
```javascript
getAppref() : string;
```
### setAppref(string) {#setAppref-string-}
```javascript
setAppref(value: string) : void;
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
