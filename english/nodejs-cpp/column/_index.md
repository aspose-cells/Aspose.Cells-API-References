---
title: Column
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents a single column in a worksheet.
type: docs
url: /nodejs-cpp/column/
---

## Column class

Represents a single column in a worksheet.

```javascript
class Column;
```


## Methods

| Method | Description |
| --- | --- |
| [getIndex()](#getIndex--)| Gets the index of this column. |
| [getWidth()](#getWidth--)| Gets and sets the column width in unit of characters. |
| [setWidth(number)](#setWidth-number-)| Gets and sets the column width in unit of characters. |
| [getGroupLevel()](#getGroupLevel--)| Gets the group level of the column. |
| [setGroupLevel(number)](#setGroupLevel-number-)| Gets the group level of the column. |
| [isHidden()](#isHidden--)| Indicates whether the column is hidden. |
| [setIsHidden(boolean)](#setIsHidden-boolean-)| Indicates whether the column is hidden. |
| [getHasCustomStyle()](#getHasCustomStyle--)| Indicates whether this column has custom style settings(different from the default one inherited from workbook). |
| [isCollapsed()](#isCollapsed--)| whether the column is collapsed |
| [setIsCollapsed(boolean)](#setIsCollapsed-boolean-)| whether the column is collapsed |
| [applyStyle(Style, StyleFlag)](#applyStyle-style-styleflag-)| Applies formats for a whole column. |
| [getStyle()](#getStyle--)| Gets the style of this column. |
| [setStyle(Style)](#setStyle-style-)| Sets the style of this column. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### getIndex() {#getIndex--}

Gets the index of this column.

```javascript
getIndex() : number;
```


### getWidth() {#getWidth--}

Gets and sets the column width in unit of characters.

```javascript
getWidth() : number;
```


**Remarks**

For spreadsheet, column width is measured as the number of characters of the maximum digit width of the numbers 0~9 as rendered in the normal style's font.

### setWidth(number) {#setWidth-number-}

Gets and sets the column width in unit of characters.

```javascript
setWidth(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

For spreadsheet, column width is measured as the number of characters of the maximum digit width of the numbers 0~9 as rendered in the normal style's font.

### getGroupLevel() {#getGroupLevel--}

Gets the group level of the column.

```javascript
getGroupLevel() : number;
```


### setGroupLevel(number) {#setGroupLevel-number-}

Gets the group level of the column.

```javascript
setGroupLevel(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### isHidden() {#isHidden--}

Indicates whether the column is hidden.

```javascript
isHidden() : boolean;
```


### setIsHidden(boolean) {#setIsHidden-boolean-}

Indicates whether the column is hidden.

```javascript
setIsHidden(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getHasCustomStyle() {#getHasCustomStyle--}

Indicates whether this column has custom style settings(different from the default one inherited from workbook).

```javascript
getHasCustomStyle() : boolean;
```


### isCollapsed() {#isCollapsed--}

whether the column is collapsed

```javascript
isCollapsed() : boolean;
```


### setIsCollapsed(boolean) {#setIsCollapsed-boolean-}

whether the column is collapsed

```javascript
setIsCollapsed(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### applyStyle(Style, StyleFlag) {#applyStyle-style-styleflag-}

Applies formats for a whole column.

```javascript
applyStyle(style: Style, flag: StyleFlag) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| style | [Style](../style/) | The style object which will be applied. |
| flag | [StyleFlag](../styleflag/) | Flags which indicates applied formatting properties. |

### getStyle() {#getStyle--}

Gets the style of this column.

```javascript
getStyle() : Style;
```


**Returns**

[Style](../style/)

**Remarks**

Modifying the returned style object directly takes no effect for this column or any cells in this column. You have to call [ApplyStyle(Style, StyleFlag)](../applystyle(style, styleflag)/) or [ApplyStyle(Style, StyleFlag)](../applystyle(style, styleflag)/) method to apply the change to this column.<br></br> Column's style is the style which will be inherited by cells in this column(those cells that have no custom style settings, such as existing cells that have not been set style explicitly, or those that have not been instantiated)

### setStyle(Style) {#setStyle-style-}

Sets the style of this column.

```javascript
setStyle(style: Style) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| style | [Style](../style/) | the style to be used as the default style for cells in this column. |

**Remarks**

This method only sets the given style as the default style for this column, without changing the style settings for existing cells in this column. To update style settings of existing cells to the specified style at the same time, please use [ApplyStyle(Style, StyleFlag)](../applystyle(style, styleflag)/)

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



