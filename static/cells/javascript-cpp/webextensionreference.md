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
