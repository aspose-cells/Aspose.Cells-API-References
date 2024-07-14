---
title: FileFontSource
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the single TrueType font file stored in the file system.
type: docs
url: /nodejs-cpp/filefontsource/
---

## FileFontSource class

Represents the single TrueType font file stored in the file system.

```javascript
class FileFontSource extends FontSourceBase;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor(FontSourceBase)](#constructor-fontsourcebase-)| Constructs from a parent object convertible to this. |
| [constructor(string)](#constructor-string-)| Ctor. |

## Methods

| Method | Description |
| --- | --- |
| [getFilePath()](#getFilePath--)| Path to font file. |
| [getType()](#getType--)| Returns the type of the font source. |


### constructor(FontSourceBase) {#constructor-fontsourcebase-}

Constructs from a parent object convertible to this.

```javascript
constructor(obj: FontSourceBase);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | FontSourceBase | The parent object. |

### constructor(string) {#constructor-string-}

Ctor.

```javascript
constructor(filePath: string);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filePath | string | path to font file |

### getFilePath() {#getFilePath--}

Path to font file.

```javascript
getFilePath() : string;
```


### getType() {#getType--}

Returns the type of the font source.

```javascript
getType() : FontSourceType;
```


**Returns**

[FontSourceType](/nodejs-cpp/fontsourcetype/)


