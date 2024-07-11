---
title: MetadataOptions
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the options of loading metadata of the file.
type: docs
url: /nodejs-cpp/metadataoptions/
---

## MetadataOptions class

Represents the options of loading metadata of the file.

```javascript
class MetadataOptions;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor(MetadataType)](#constructor-metadatatype-)| Creates an options of loading the metadata. |

## Methods

| Method | Description |
| --- | --- |
| [getMetadataType()](#getMetadataType--)| Gets and sets the type of the metadata which is loading. |
| [getPassword()](#getPassword--)| Represents Workbook file encryption password. |
| [setPassword(string)](#setPassword-string-)| Represents Workbook file encryption password. |
| [getKeyLength()](#getKeyLength--)| The key length. |
| [setKeyLength(number)](#setKeyLength-number-)| The key length. |


### constructor(MetadataType) {#constructor-metadatatype-}

Creates an options of loading the metadata.

```javascript
constructor(metadataType: MetadataType);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| metadataType | [MetadataType](./metadatatype/) | The type of metadata. |

### getMetadataType() {#getMetadataType--}

Gets and sets the type of the metadata which is loading.

```javascript
getMetadataType() : MetadataType;
```


**Returns**

[MetadataType](./metadatatype/)

### getPassword() {#getPassword--}

Represents Workbook file encryption password.

```javascript
getPassword() : string;
```


### setPassword(string) {#setPassword-string-}

Represents Workbook file encryption password.

```javascript
setPassword(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getKeyLength() {#getKeyLength--}

The key length.

```javascript
getKeyLength() : number;
```


### setKeyLength(number) {#setKeyLength-number-}

The key length.

```javascript
setKeyLength(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |


