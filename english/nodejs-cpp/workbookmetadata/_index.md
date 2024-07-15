---
title: WorkbookMetadata
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the meta data.
type: docs
url: /nodejs-cpp/workbookmetadata/
---

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

## Methods

| Method | Description |
| --- | --- |
| [getOptions()](#getOptions--)| Gets the options of the metadata. |
| [getBuiltInDocumentProperties()](#getBuiltInDocumentProperties--)| Returns a [DocumentProperty](../documentproperty/) collection that represents all the  built-in document properties of the spreadsheet. |
| [getCustomDocumentProperties()](#getCustomDocumentProperties--)| Returns a [DocumentProperty](../documentproperty/) collection that represents all the custom document properties of the spreadsheet. |
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

### getOptions() {#getOptions--}

Gets the options of the metadata.

```javascript
getOptions() : MetadataOptions;
```


**Returns**

[MetadataOptions](../metadataoptions/)

### getBuiltInDocumentProperties() {#getBuiltInDocumentProperties--}

Returns a [DocumentProperty](../documentproperty/) collection that represents all the  built-in document properties of the spreadsheet.

```javascript
getBuiltInDocumentProperties() : BuiltInDocumentPropertyCollection;
```


**Returns**

[BuiltInDocumentPropertyCollection](../builtindocumentpropertycollection/)

### getCustomDocumentProperties() {#getCustomDocumentProperties--}

Returns a [DocumentProperty](../documentproperty/) collection that represents all the custom document properties of the spreadsheet.

```javascript
getCustomDocumentProperties() : CustomDocumentPropertyCollection;
```


**Returns**

[CustomDocumentPropertyCollection](../customdocumentpropertycollection/)

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


