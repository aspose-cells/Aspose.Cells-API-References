---
title: FontSetting
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents a range of characters within the cell text.
type: docs
url: /nodejs-cpp/fontsetting/
---

## FontSetting class

Represents a range of characters within the cell text.

```javascript
class FontSetting;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor(number, number, WorksheetCollection)](#constructor-number-number-worksheetcollection-)|  |

## Methods

| Method | Description |
| --- | --- |
| [getStartIndex()](#getStartIndex--)| Gets the start index of the characters. |
| [getLength()](#getLength--)| Gets the length of the characters. |
| [getFont()](#getFont--)| Returns the font of this object. |
| [getTextOptions()](#getTextOptions--)| Returns the text options. |
| [setWordArtStyle(PresetWordArtStyle)](#setWordArtStyle-presetwordartstyle-)| Sets the preset WordArt style. |
| [getType()](#getType--)| Gets the type of text node. |


### constructor(number, number, WorksheetCollection) {#constructor-number-number-worksheetcollection-}



```javascript
constructor(startIndex: number, length: number, sheets: WorksheetCollection);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | number |  |
| length | number |  |
| sheets | [WorksheetCollection](../worksheetcollection/) |  |

### getStartIndex() {#getStartIndex--}

Gets the start index of the characters.

```javascript
getStartIndex() : number;
```


### getLength() {#getLength--}

Gets the length of the characters.

```javascript
getLength() : number;
```


### getFont() {#getFont--}

Returns the font of this object.

```javascript
getFont() : Font;
```


**Returns**

[Font](../font/)

### getTextOptions() {#getTextOptions--}

Returns the text options.

```javascript
getTextOptions() : TextOptions;
```


**Returns**

[TextOptions](../textoptions/)

### setWordArtStyle(PresetWordArtStyle) {#setWordArtStyle-presetwordartstyle-}

Sets the preset WordArt style.

```javascript
setWordArtStyle(style: PresetWordArtStyle) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| style | [PresetWordArtStyle](../presetwordartstyle/) | The preset WordArt style. |

**Remarks**

Only for the text of shape/chart.

### getType() {#getType--}

Gets the type of text node.

```javascript
getType() : TextNodeType;
```


**Returns**

[TextNodeType](../textnodetype/)


