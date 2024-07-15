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
| [constructor(number[])](#constructor-numberarray-)| Ctor. |

## Methods

| Method | Description |
| --- | --- |
| [getFontData()](#getFontData--)| Binary font data. |
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

### constructor(number[]) {#constructor-numberarray-}

Ctor.

```javascript
constructor(fontData: number[]);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fontData | number[] | Binary font data. |

### getFontData() {#getFontData--}

Binary font data.

```javascript
getFontData() : number[];
```


**Returns**

number[]

### getType() {#getType--}

Returns the type of the font source.

```javascript
getType() : FontSourceType;
```


**Returns**

[FontSourceType](../fontsourcetype/)


