##WebExtension
Represents an Office Addin instance.
## WebExtension class
Represents an Office Add-in instance.
```javascript
class WebExtension;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [id](#id--)| string | Gets and sets the uniquely identifies the Office Add-in instance in the current document. |
| [isFrozen](#isFrozen--)| boolean | Indicates whether the user can interact with the Office Add-in or not. |
| [reference](#reference--)| WebExtensionReference | Readonly. Get the primary reference to an Office Add-in. |
| [alterReferences](#alterReferences--)| WebExtensionReferenceCollection | Readonly. Gets a list of alter references. |
| [properties](#properties--)| WebExtensionPropertyCollection | Readonly. Gets all properties of web extension. |
| [bindings](#bindings--)| WebExtensionBindingCollection | Readonly. Gets all bindings relationship between an Office Add-in and the data in the document. |
## Methods
| Method | Description |
| --- | --- |
| [getId()](#getId--)| <b>@deprecated.</b> Please use the 'id' property instead. Gets and sets the uniquely identifies the Office Add-in instance in the current document. |
| [setId(string)](#setId-string-)| <b>@deprecated.</b> Please use the 'id' property instead. Gets and sets the uniquely identifies the Office Add-in instance in the current document. |
| [isFrozen()](#isFrozen--)| <b>@deprecated.</b> Please use the 'isFrozen' property instead. Indicates whether the user can interact with the Office Add-in or not. |
| [setIsFrozen(boolean)](#setIsFrozen-boolean-)| <b>@deprecated.</b> Please use the 'isFrozen' property instead. Indicates whether the user can interact with the Office Add-in or not. |
| [getReference()](#getReference--)| <b>@deprecated.</b> Please use the 'reference' property instead. Get the primary reference to an Office Add-in. |
| [getAlterReferences()](#getAlterReferences--)| <b>@deprecated.</b> Please use the 'alterReferences' property instead. Gets a list of alter references. |
| [getProperties()](#getProperties--)| <b>@deprecated.</b> Please use the 'properties' property instead. Gets all properties of web extension. |
| [getBindings()](#getBindings--)| <b>@deprecated.</b> Please use the 'bindings' property instead. Gets all bindings relationship between an Office Add-in and the data in the document. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### id {#id--}
Gets and sets the uniquely identifies the Office Add-in instance in the current document.
```javascript
id : string;
```
### isFrozen {#isFrozen--}
Indicates whether the user can interact with the Office Add-in or not.
```javascript
isFrozen : boolean;
```
### reference {#reference--}
Readonly. Get the primary reference to an Office Add-in.
```javascript
reference : WebExtensionReference;
```
### alterReferences {#alterReferences--}
Readonly. Gets a list of alter references.
```javascript
alterReferences : WebExtensionReferenceCollection;
```
### properties {#properties--}
Readonly. Gets all properties of web extension.
```javascript
properties : WebExtensionPropertyCollection;
```
### bindings {#bindings--}
Readonly. Gets all bindings relationship between an Office Add-in and the data in the document.
```javascript
bindings : WebExtensionBindingCollection;
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
### isFrozen() {#isFrozen--}
```javascript
isFrozen() : boolean;
```
### setIsFrozen(boolean) {#setIsFrozen-boolean-}
```javascript
setIsFrozen(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getReference() {#getReference--}
```javascript
getReference() : WebExtensionReference;
```
**Returns**
[WebExtensionReference](../webextensionreference/)
### getAlterReferences() {#getAlterReferences--}
```javascript
getAlterReferences() : WebExtensionReferenceCollection;
```
**Returns**
[WebExtensionReferenceCollection](../webextensionreferencecollection/)
### getProperties() {#getProperties--}
```javascript
getProperties() : WebExtensionPropertyCollection;
```
**Returns**
[WebExtensionPropertyCollection](../webextensionpropertycollection/)
### getBindings() {#getBindings--}
```javascript
getBindings() : WebExtensionBindingCollection;
```
**Returns**
[WebExtensionBindingCollection](../webextensionbindingcollection/)
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
