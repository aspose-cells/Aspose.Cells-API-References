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

| Constructor | Description |
| --- | --- |
| [constructor(FontSourceBase)](#constructor-fontsourcebase-)| Constructs from a parent object convertible to this. |
| [constructor(Uint8Array)](#constructor-uint8array-)| Ctor. |

## Properties

| Property | Type | Description |
| --- | --- | --- |
| [fontData](#fontData--)| Uint8Array | Readonly. Binary font data. |
| [type](#type--)| FontSourceType | Readonly. Returns the type of the font source. |

## Methods

| Method | Description |
| --- | --- |
| [getFontData()](#getFontData--)| <b>@deprecated.</b> Please use the 'fontData' property instead. Binary font data. |
| [getType()](#getType--)| <b>@deprecated.</b> Please use the 'type' property instead. Returns the type of the font source. |
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

### fontData {#fontData--}

Readonly. Binary font data.

```javascript
fontData : Uint8Array;
```


### type {#type--}

Readonly. Returns the type of the font source.

```javascript
type : FontSourceType;
```


### getFontData() {#getFontData--}

<b>@deprecated.</b> Please use the 'fontData' property instead. Binary font data.

```javascript
getFontData() : Uint8Array;
```


### getType() {#getType--}

<b>@deprecated.</b> Please use the 'type' property instead. Returns the type of the font source.

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



