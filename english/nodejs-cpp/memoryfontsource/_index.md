---
title: MemoryFontSource
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the single TrueType font file stored in memory.
type: docs
url: /nodejs-cpp/memoryfontsource/
---

## MemoryFontSource class

Represents the single TrueType font file stored in memory.

```javascript
class MemoryFontSource extends FontSourceBase;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor(FontSourceBase)](#constructor-fontsourcebase-)| Constructs from a parent object convertible to this. |
| [constructor(Uint8Array)](#constructor-uint8array-)| Ctor. |

## Methods

| Method | Description |
| --- | --- |
| [getFontData()](#getFontData--)| Binary font data. |
| [getType()](#getType--)| Returns the type of the font source. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### constructor(FontSourceBase) {#constructor-fontsourcebase-}

Constructs from a parent object convertible to this.

```javascript
constructor(obj: FontSourceBase);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | FontSourceBase | The parent object. |

### constructor(Uint8Array) {#constructor-uint8array-}

Ctor.

```javascript
constructor(fontData: Uint8Array);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fontData | number[] | Binary font data. |

### getFontData() {#getFontData--}

Binary font data.

```javascript
getFontData() : Uint8Array;
```


### getType() {#getType--}

Returns the type of the font source.

```javascript
getType() : FontSourceType;
```


**Returns**

[FontSourceType](../fontsourcetype/)

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



