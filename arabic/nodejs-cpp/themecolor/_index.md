---
title: ThemeColor
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents a theme color.
type: docs
url: /ar/nodejs-cpp/themecolor/
---

## ThemeColor class

Represents a theme color.

```javascript
class ThemeColor;
```


### Example
```javascript
const { Workbook, ThemeColor, ThemeColorType, BackgroundType } = require("aspose.cells.node");

//إنشاء كائن Workbook.
var workbook = new Workbook();
var cells = workbook.worksheets.get(0).cells;
cells.get("A1").putValue("Hello World");
var style = cells.get("A1").getStyle();
//ضبط نوع لون ThemeColorType.Text2 مع إضاءة بنسبة 40% كلون الخط.
style.font.themeColor = new ThemeColor(ThemeColorType.Text2, 0.4);
style.pattern = BackgroundType.Solid;
//ضبط نوع لون ThemeColorType.Background2 مع تعتيم بنسبة 75% كلون المقدمة
style.foregroundThemeColor = new ThemeColor(ThemeColorType.Background2, -0.75);
cells.get("A1").setStyle(style);
//حفظ ملف Excel
workbook.save("output/ThemeColor.xlsx");
```
## Constructors

| Constructor | Description |
| --- | --- |
| [constructor(ThemeColorType, number)](#constructor-themecolortype-number-)|  |

## Properties

| Property | Type | Description |
| --- | --- | --- |
| [colorType](#colorType--)| ThemeColorType | Gets and sets the theme type. |
| [tint](#tint--)| number | Gets and sets the tint value. |

## Methods

| Method | Description |
| --- | --- |
| [getColorType()](#getColorType--)| <b>@deprecated.</b> Please use the 'colorType' property instead. Gets and sets the theme type. |
| [setColorType(ThemeColorType)](#setColorType-themecolortype-)| <b>@deprecated.</b> Please use the 'colorType' property instead. Gets and sets the theme type. |
| [getTint()](#getTint--)| <b>@deprecated.</b> Please use the 'tint' property instead. Gets and sets the tint value. |
| [setTint(number)](#setTint-number-)| <b>@deprecated.</b> Please use the 'tint' property instead. Gets and sets the tint value. |
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

### colorType {#colorType--}

Gets and sets the theme type.

```javascript
colorType : ThemeColorType;
```


### tint {#tint--}

Gets and sets the tint value.

```javascript
tint : number;
```


**Remarks**

The tint value is stored as a double from -1.0 to 1.0, where -1.0 means 100% darken and 1.0 means 100% lighten. Also, 0.0 means no change.

### getColorType() {#getColorType--}

<b>@deprecated.</b> Please use the 'colorType' property instead. Gets and sets the theme type.

```javascript
getColorType() : ThemeColorType;
```


**Returns**

[ThemeColorType](../themecolortype/)

### setColorType(ThemeColorType) {#setColorType-themecolortype-}

<b>@deprecated.</b> Please use the 'colorType' property instead. Gets and sets the theme type.

```javascript
setColorType(value: ThemeColorType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ThemeColorType](../themecolortype/) | The value to set. |

### getTint() {#getTint--}

<b>@deprecated.</b> Please use the 'tint' property instead. Gets and sets the tint value.

```javascript
getTint() : number;
```


**Remarks**

The tint value is stored as a double from -1.0 to 1.0, where -1.0 means 100% darken and 1.0 means 100% lighten. Also, 0.0 means no change.

### setTint(number) {#setTint-number-}

<b>@deprecated.</b> Please use the 'tint' property instead. Gets and sets the tint value.

```javascript
setTint(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

The tint value is stored as a double from -1.0 to 1.0, where -1.0 means 100% darken and 1.0 means 100% lighten. Also, 0.0 means no change.

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



