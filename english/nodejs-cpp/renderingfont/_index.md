---
title: RenderingFont
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Font for rendering.
type: docs
url: /nodejs-cpp/renderingfont/
---

## RenderingFont class

Font for rendering.

```javascript
class RenderingFont;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor(string, number)](#constructor-string-number-)| Initializes a new instance of the [RenderingFont](../renderingfont/) |

## Methods

| Method | Description |
| --- | --- |
| [getName()](#getName--)| Gets name of the font. |
| [getSize()](#getSize--)| Gets size of the font in points. |
| [getBold()](#getBold--)| Gets or sets bold for the font. |
| [setBold(boolean)](#setBold-boolean-)| Gets or sets bold for the font. |
| [getItalic()](#getItalic--)| Gets or sets italic for the font. |
| [setItalic(boolean)](#setItalic-boolean-)| Gets or sets italic for the font. |
| [getColor()](#getColor--)| Gets or sets color for the font. |
| [setColor(Color)](#setColor-color-)| Gets or sets color for the font. |


### constructor(string, number) {#constructor-string-number-}

Initializes a new instance of the [RenderingFont](../renderingfont/)

```javascript
constructor(fontName: string, fontSize: number);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fontName | string | font name |
| fontSize | number | font size in points |

### getName() {#getName--}

Gets name of the font.

```javascript
getName() : string;
```


### getSize() {#getSize--}

Gets size of the font in points.

```javascript
getSize() : number;
```


### getBold() {#getBold--}

Gets or sets bold for the font.

```javascript
getBold() : boolean;
```


### setBold(boolean) {#setBold-boolean-}

Gets or sets bold for the font.

```javascript
setBold(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getItalic() {#getItalic--}

Gets or sets italic for the font.

```javascript
getItalic() : boolean;
```


### setItalic(boolean) {#setItalic-boolean-}

Gets or sets italic for the font.

```javascript
setItalic(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getColor() {#getColor--}

Gets or sets color for the font.

```javascript
getColor() : Color;
```


**Returns**

[Color](../color/)

### setColor(Color) {#setColor-color-}

Gets or sets color for the font.

```javascript
setColor(value: Color) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../color/) | The value to set. |


