##WebExtensionReference
Represents identify the provider location and version of the extension.
## WebExtensionReference class
Represents identify the provider location and version of the extension.
```javascript
class WebExtensionReference;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [id](#id--)| string | Gets and sets the identifier associated with the Office Add-in within a catalog provider. The identifier MUST be unique within a catalog provider. |
| [version](#version--)| string | Gets and sets the version. |
| [storeName](#storeName--)| string | Gets and sets the instance of the marketplace where the Office Add-in is stored. . |
| [storeType](#storeType--)| WebExtensionStoreType | Gets and sets the type of marketplace that the store attribute identifies. |
## Methods
| Method | Description |
| --- | --- |
| [getId()](#getId--)| <b>@deprecated.</b> Please use the 'id' property instead. Gets and sets the identifier associated with the Office Add-in within a catalog provider. The identifier MUST be unique within a catalog provider. |
| [setId(string)](#setId-string-)| <b>@deprecated.</b> Please use the 'id' property instead. Gets and sets the identifier associated with the Office Add-in within a catalog provider. The identifier MUST be unique within a catalog provider. |
| [getVersion()](#getVersion--)| <b>@deprecated.</b> Please use the 'version' property instead. Gets and sets the version. |
| [setVersion(string)](#setVersion-string-)| <b>@deprecated.</b> Please use the 'version' property instead. Gets and sets the version. |
| [getStoreName()](#getStoreName--)| <b>@deprecated.</b> Please use the 'storeName' property instead. Gets and sets the instance of the marketplace where the Office Add-in is stored. . |
| [setStoreName(string)](#setStoreName-string-)| <b>@deprecated.</b> Please use the 'storeName' property instead. Gets and sets the instance of the marketplace where the Office Add-in is stored. . |
| [getStoreType()](#getStoreType--)| <b>@deprecated.</b> Please use the 'storeType' property instead. Gets and sets the type of marketplace that the store attribute identifies. |
| [setStoreType(WebExtensionStoreType)](#setStoreType-webextensionstoretype-)| <b>@deprecated.</b> Please use the 'storeType' property instead. Gets and sets the type of marketplace that the store attribute identifies. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### id {#id--}
Gets and sets the identifier associated with the Office Add-in within a catalog provider. The identifier MUST be unique within a catalog provider.
```javascript
id : string;
```
### version {#version--}
Gets and sets the version.
```javascript
version : string;
```
### storeName {#storeName--}
Gets and sets the instance of the marketplace where the Office Add-in is stored. .
```javascript
storeName : string;
```
### storeType {#storeType--}
Gets and sets the type of marketplace that the store attribute identifies.
```javascript
storeType : WebExtensionStoreType;
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
### getVersion() {#getVersion--}
```javascript
getVersion() : string;
```
### setVersion(string) {#setVersion-string-}
```javascript
setVersion(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getStoreName() {#getStoreName--}
```javascript
getStoreName() : string;
```
### setStoreName(string) {#setStoreName-string-}
```javascript
setStoreName(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getStoreType() {#getStoreType--}
```javascript
getStoreType() : WebExtensionStoreType;
```
**Returns**
[WebExtensionStoreType](../webextensionstoretype/)
### setStoreType(WebExtensionStoreType) {#setStoreType-webextensionstoretype-}
```javascript
setStoreType(value: WebExtensionStoreType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [WebExtensionStoreType](../webextensionstoretype/) | The value to set. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
