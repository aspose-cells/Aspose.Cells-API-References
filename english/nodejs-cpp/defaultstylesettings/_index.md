---
title: DefaultStyleSettings
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Settings for the default values of workbooks style properties.
type: docs
url: /nodejs-cpp/defaultstylesettings/
---

## DefaultStyleSettings class

Settings for the default values of workbook's style properties.

```javascript
class DefaultStyleSettings;
```


## Methods

| Method | Description |
| --- | --- |
| [getBuiltInPreference()](#getBuiltInPreference--)| Indicates whether property for number format is preferrable when the style defines both built-in number and custom pattern. Default value is false, that means by default custom pattern will be used to format values as long as it is not empty for one style. |
| [setBuiltInPreference(boolean)](#setBuiltInPreference-boolean-)| Indicates whether property for number format is preferrable when the style defines both built-in number and custom pattern. Default value is false, that means by default custom pattern will be used to format values as long as it is not empty for one style. |
| [getFontName()](#getFontName--)| Gets/Sets the default font name for the workbook |
| [setFontName(string)](#setFontName-string-)| Gets/Sets the default font name for the workbook |
| [getFontSize()](#getFontSize--)| Gets/Sets the default standard font size for the workbook. |
| [setFontSize(number)](#setFontSize-number-)| Gets/Sets the default standard font size for the workbook. |
| [getHorizontalAlignment()](#getHorizontalAlignment--)| Gets/Sets the default value for horizontal alignment |
| [setHorizontalAlignment(TextAlignmentType)](#setHorizontalAlignment-textalignmenttype-)| Gets/Sets the default value for horizontal alignment |
| [getVerticalAlignment()](#getVerticalAlignment--)| Gets/Sets the default value for vertical alignment |
| [setVerticalAlignment(TextAlignmentType)](#setVerticalAlignment-textalignmenttype-)| Gets/Sets the default value for vertical alignment |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### getBuiltInPreference() {#getBuiltInPreference--}

Indicates whether property for number format is preferrable when the style defines both built-in number and custom pattern. Default value is false, that means by default custom pattern will be used to format values as long as it is not empty for one style.

```javascript
getBuiltInPreference() : boolean;
```


**Remarks**

When loading workbook from existing template file, maybe both built-in number and custom pattern are defined for one style. This property determine whether we should use the built-in number or the custom pattern when formatting values with the style.

### setBuiltInPreference(boolean) {#setBuiltInPreference-boolean-}

Indicates whether property for number format is preferrable when the style defines both built-in number and custom pattern. Default value is false, that means by default custom pattern will be used to format values as long as it is not empty for one style.

```javascript
setBuiltInPreference(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

When loading workbook from existing template file, maybe both built-in number and custom pattern are defined for one style. This property determine whether we should use the built-in number or the custom pattern when formatting values with the style.

### getFontName() {#getFontName--}

Gets/Sets the default font name for the workbook

```javascript
getFontName() : string;
```


### setFontName(string) {#setFontName-string-}

Gets/Sets the default font name for the workbook

```javascript
setFontName(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getFontSize() {#getFontSize--}

Gets/Sets the default standard font size for the workbook.

```javascript
getFontSize() : number;
```


### setFontSize(number) {#setFontSize-number-}

Gets/Sets the default standard font size for the workbook.

```javascript
setFontSize(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getHorizontalAlignment() {#getHorizontalAlignment--}

Gets/Sets the default value for horizontal alignment

```javascript
getHorizontalAlignment() : TextAlignmentType;
```


**Returns**

[TextAlignmentType](../textalignmenttype/)

### setHorizontalAlignment(TextAlignmentType) {#setHorizontalAlignment-textalignmenttype-}

Gets/Sets the default value for horizontal alignment

```javascript
setHorizontalAlignment(value: TextAlignmentType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextAlignmentType](../textalignmenttype/) | The value to set. |

### getVerticalAlignment() {#getVerticalAlignment--}

Gets/Sets the default value for vertical alignment

```javascript
getVerticalAlignment() : TextAlignmentType;
```


**Returns**

[TextAlignmentType](../textalignmenttype/)

### setVerticalAlignment(TextAlignmentType) {#setVerticalAlignment-textalignmenttype-}

Gets/Sets the default value for vertical alignment

```javascript
setVerticalAlignment(value: TextAlignmentType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextAlignmentType](../textalignmenttype/) | The value to set. |

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



