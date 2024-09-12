---
title: ThemeColor
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents a theme color.
type: docs
url: /nodejs-cpp/themecolor/
---

## ThemeColor class

Represents a theme color.

```javascript
class ThemeColor;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor(ThemeColorType, number)](#constructor-themecolortype-number-)|  |

## Methods

| Method | Description |
| --- | --- |
| [getColorType()](#getColorType--)| Gets and sets the theme type. |
| [setColorType(ThemeColorType)](#setColorType-themecolortype-)| Gets and sets the theme type. |
| [getTint()](#getTint--)| Gets and sets the tint value. |
| [setTint(number)](#setTint-number-)| Gets and sets the tint value. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### constructor(ThemeColorType, number) {#constructor-themecolortype-number-}



```javascript
constructor(type: ThemeColorType, tint: number);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [ThemeColorType](../themecolortype/) | The theme type. |
| tint | number | The tint value. |

### getColorType() {#getColorType--}

Gets and sets the theme type.

```javascript
getColorType() : ThemeColorType;
```


**Returns**

[ThemeColorType](../themecolortype/)

### setColorType(ThemeColorType) {#setColorType-themecolortype-}

Gets and sets the theme type.

```javascript
setColorType(value: ThemeColorType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ThemeColorType](../themecolortype/) | The value to set. |

### getTint() {#getTint--}

Gets and sets the tint value.

```javascript
getTint() : number;
```


**Remarks**

The tint value is stored as a double from -1.0 .. 1.0, where -1.0 means 100% darken and 1.0 means 100% lighten. Also, 0.0 means no change.

### setTint(number) {#setTint-number-}

Gets and sets the tint value.

```javascript
setTint(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

The tint value is stored as a double from -1.0 .. 1.0, where -1.0 means 100% darken and 1.0 means 100% lighten. Also, 0.0 means no change.

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



