##WorkbookMetadata
Represents the meta data.
## WorkbookMetadata class
Represents the meta data.
```javascript
class WorkbookMetadata;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor(string, MetadataOptions)](#constructor-string-metadataoptions-)| Create the meta data object. |
| [constructor(Uint8Array, MetadataOptions)](#constructor-uint8array-metadataoptions-)| Create the meta data object. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [options](#options--)| MetadataOptions | Readonly. Gets the options of the metadata. |
| [builtInDocumentProperties](#builtInDocumentProperties--)| BuiltInDocumentPropertyCollection | Readonly. Returns a [DocumentProperty](../documentproperty/) collection that represents all the  built-in document properties of the spreadsheet. |
| [customDocumentProperties](#customDocumentProperties--)| CustomDocumentPropertyCollection | Readonly. Returns a [DocumentProperty](../documentproperty/) collection that represents all the custom document properties of the spreadsheet. |
## Methods
| Method | Description |
| --- | --- |
| [save(string)](#save-string-)| Save the modified metadata to the file. |
| [save(Uint8Array)](#save-uint8array-)| Save the modified metadata to the stream. |
### constructor(string, MetadataOptions) {#constructor-string-metadataoptions-}
Create the meta data object.
```javascript
constructor(fileName: string, options: MetadataOptions);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | string |  |
| options | [MetadataOptions](../metadataoptions/) |  |
### constructor(Uint8Array, MetadataOptions) {#constructor-uint8array-metadataoptions-}
Create the meta data object.
```javascript
constructor(stream: Uint8Array, options: MetadataOptions);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | Uint8Array |  |
| options | [MetadataOptions](../metadataoptions/) |  |
### options {#options--}
Readonly. Gets the options of the metadata.
```javascript
options : MetadataOptions;
```
### builtInDocumentProperties {#builtInDocumentProperties--}
Readonly. Returns a [DocumentProperty](../documentproperty/) collection that represents all the  built-in document properties of the spreadsheet.
```javascript
builtInDocumentProperties : BuiltInDocumentPropertyCollection;
```
### customDocumentProperties {#customDocumentProperties--}
Readonly. Returns a [DocumentProperty](../documentproperty/) collection that represents all the custom document properties of the spreadsheet.
```javascript
customDocumentProperties : CustomDocumentPropertyCollection;
```
### save(string) {#save-string-}
Save the modified metadata to the file.
```javascript
save(fileName: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | string | The file name. |
### save(Uint8Array) {#save-uint8array-}
Save the modified metadata to the stream.
```javascript
save(stream: Uint8Array) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | Uint8Array | The stream. |
