﻿---
title: TextOptions
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the text options.
type: docs
url: /nodejs-cpp/textoptions/
---

## TextOptions class

Represents the text options.

```javascript
class TextOptions extends Font;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor(Font)](#constructor-font-)| Constructs from a parent object convertible to this. |

## Methods

| Method | Description |
| --- | --- |
| [getName()](#getName--)| Gets and sets the name of the shape. |
| [setName(string)](#setName-string-)| Gets and sets the name of the shape. |
| [getLanguageCode()](#getLanguageCode--)| Gets and sets the user interface language. |
| [setLanguageCode(CountryCode)](#setLanguageCode-countrycode-)| Gets and sets the user interface language. |
| [getLatinName()](#getLatinName--)| Gets and sets the latin name. |
| [setLatinName(string)](#setLatinName-string-)| Gets and sets the latin name. |
| [getFarEastName()](#getFarEastName--)| Gets and sets the FarEast name. |
| [setFarEastName(string)](#setFarEastName-string-)| Gets and sets the FarEast name. |
| [getFill()](#getFill--)| Represents the fill format of the text. |
| [getOutline()](#getOutline--)| Represents the outline format of the text. |
| [getShadow()](#getShadow--)| Represents a [ShadowEffect](../shadoweffect/) object that specifies shadow effect for the chart element or shape. |
| [getUnderlineColor()](#getUnderlineColor--)| Gets or sets the color of underline. |
| [setUnderlineColor(CellsColor)](#setUnderlineColor-cellscolor-)| Gets or sets the color of underline. |
| [getKerning()](#getKerning--)| Specifies the minimum font size at which character kerning will occur for this text run. |
| [setKerning(number)](#setKerning-number-)| Specifies the minimum font size at which character kerning will occur for this text run. |
| [getSpacing()](#getSpacing--)| Specifies the spacing between characters within a text run. |
| [setSpacing(number)](#setSpacing-number-)| Specifies the spacing between characters within a text run. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [getCharset()](#getCharset--)| Represent the character set. |
| [setCharset(number)](#setCharset-number-)| Represent the character set. |
| [isItalic()](#isItalic--)| Gets or sets a value indicating whether the font is italic. |
| [setIsItalic(boolean)](#setIsItalic-boolean-)| Gets or sets a value indicating whether the font is italic. |
| [isBold()](#isBold--)| Gets or sets a value indicating whether the font is bold. |
| [setIsBold(boolean)](#setIsBold-boolean-)| Gets or sets a value indicating whether the font is bold. |
| [getCapsType()](#getCapsType--)| Gets and sets the text caps type. |
| [setCapsType(TextCapsType)](#setCapsType-textcapstype-)| Gets and sets the text caps type. |
| [getStrikeType()](#getStrikeType--)| Gets the strike type of the text. |
| [setStrikeType(TextStrikeType)](#setStrikeType-textstriketype-)| Gets the strike type of the text. |
| [isStrikeout()](#isStrikeout--)| Gets or sets a value indicating whether the font is single strikeout. |
| [setIsStrikeout(boolean)](#setIsStrikeout-boolean-)| Gets or sets a value indicating whether the font is single strikeout. |
| [getScriptOffset()](#getScriptOffset--)| Gets and sets the script offset,in unit of percentage |
| [setScriptOffset(number)](#setScriptOffset-number-)| Gets and sets the script offset,in unit of percentage |
| [isSuperscript()](#isSuperscript--)| Gets or sets a value indicating whether the font is super script. |
| [setIsSuperscript(boolean)](#setIsSuperscript-boolean-)| Gets or sets a value indicating whether the font is super script. |
| [isSubscript()](#isSubscript--)| Gets or sets a value indicating whether the font is subscript. |
| [setIsSubscript(boolean)](#setIsSubscript-boolean-)| Gets or sets a value indicating whether the font is subscript. |
| [getUnderline()](#getUnderline--)| Gets or sets the font underline type. |
| [setUnderline(FontUnderlineType)](#setUnderline-fontunderlinetype-)| Gets or sets the font underline type. |
| [getDoubleSize()](#getDoubleSize--)| Gets and sets the double size of the font. |
| [setDoubleSize(number)](#setDoubleSize-number-)| Gets and sets the double size of the font. |
| [getSize()](#getSize--)| Gets or sets the size of the font. |
| [setSize(number)](#setSize-number-)| Gets or sets the size of the font. |
| [getThemeColor()](#getThemeColor--)| Gets and sets the theme color. |
| [setThemeColor(ThemeColor)](#setThemeColor-themecolor-)| Gets and sets the theme color. |
| [getColor()](#getColor--)| Gets or sets the [Color](../color/) of the font. |
| [setColor(Color)](#setColor-color-)| Gets or sets the [Color](../color/) of the font. |
| [getArgbColor()](#getArgbColor--)| Gets and sets the color with a 32-bit ARGB value. |
| [setArgbColor(number)](#setArgbColor-number-)| Gets and sets the color with a 32-bit ARGB value. |
| [isNormalizeHeights()](#isNormalizeHeights--)| Indicates whether the normalization of height that is to be applied to the text run. |
| [setIsNormalizeHeights(boolean)](#setIsNormalizeHeights-boolean-)| Indicates whether the normalization of height that is to be applied to the text run. |
| [getSchemeType()](#getSchemeType--)| Gets and sets the scheme type of the font. |
| [setSchemeType(FontSchemeType)](#setSchemeType-fontschemetype-)| Gets and sets the scheme type of the font. |
| [equals(Font)](#equals-font-)| Checks if two fonts are equals. |
| [toString()](#toString--)| Returns a string represents the current Cell object. |


### constructor(Font) {#constructor-font-}

Constructs from a parent object convertible to this.

```javascript
constructor(obj: Font);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | Font | The parent object. |

### getName() {#getName--}

Gets and sets the name of the shape.

```javascript
getName() : string;
```


### setName(string) {#setName-string-}

Gets and sets the name of the shape.

```javascript
setName(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getLanguageCode() {#getLanguageCode--}

Gets and sets the user interface language.

```javascript
getLanguageCode() : CountryCode;
```


**Returns**

[CountryCode](../countrycode/)

### setLanguageCode(CountryCode) {#setLanguageCode-countrycode-}

Gets and sets the user interface language.

```javascript
setLanguageCode(value: CountryCode) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CountryCode](../countrycode/) | The value to set. |

### getLatinName() {#getLatinName--}

Gets and sets the latin name.

```javascript
getLatinName() : string;
```


### setLatinName(string) {#setLatinName-string-}

Gets and sets the latin name.

```javascript
setLatinName(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getFarEastName() {#getFarEastName--}

Gets and sets the FarEast name.

```javascript
getFarEastName() : string;
```


### setFarEastName(string) {#setFarEastName-string-}

Gets and sets the FarEast name.

```javascript
setFarEastName(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getFill() {#getFill--}

Represents the fill format of the text.

```javascript
getFill() : FillFormat;
```


**Returns**

[FillFormat](../fillformat/)

### getOutline() {#getOutline--}

Represents the outline format of the text.

```javascript
getOutline() : LineFormat;
```


**Returns**

[LineFormat](../lineformat/)

### getShadow() {#getShadow--}

Represents a [ShadowEffect](../shadoweffect/) object that specifies shadow effect for the chart element or shape.

```javascript
getShadow() : ShadowEffect;
```


**Returns**

[ShadowEffect](../shadoweffect/)

### getUnderlineColor() {#getUnderlineColor--}

Gets or sets the color of underline.

```javascript
getUnderlineColor() : CellsColor;
```


**Returns**

[CellsColor](../cellscolor/)

### setUnderlineColor(CellsColor) {#setUnderlineColor-cellscolor-}

Gets or sets the color of underline.

```javascript
setUnderlineColor(value: CellsColor) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CellsColor](../cellscolor/) | The value to set. |

### getKerning() {#getKerning--}

Specifies the minimum font size at which character kerning will occur for this text run.

```javascript
getKerning() : number;
```


### setKerning(number) {#setKerning-number-}

Specifies the minimum font size at which character kerning will occur for this text run.

```javascript
setKerning(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getSpacing() {#getSpacing--}

Specifies the spacing between characters within a text run.

```javascript
getSpacing() : number;
```


### setSpacing(number) {#setSpacing-number-}

Specifies the spacing between characters within a text run.

```javascript
setSpacing(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```


### getCharset() {#getCharset--}

Represent the character set.

```javascript
getCharset() : number;
```


### setCharset(number) {#setCharset-number-}

Represent the character set.

```javascript
setCharset(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### isItalic() {#isItalic--}

Gets or sets a value indicating whether the font is italic.

```javascript
isItalic() : boolean;
```


### setIsItalic(boolean) {#setIsItalic-boolean-}

Gets or sets a value indicating whether the font is italic.

```javascript
setIsItalic(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isBold() {#isBold--}

Gets or sets a value indicating whether the font is bold.

```javascript
isBold() : boolean;
```


### setIsBold(boolean) {#setIsBold-boolean-}

Gets or sets a value indicating whether the font is bold.

```javascript
setIsBold(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getCapsType() {#getCapsType--}

Gets and sets the text caps type.

```javascript
getCapsType() : TextCapsType;
```


**Returns**

[TextCapsType](../textcapstype/)

### setCapsType(TextCapsType) {#setCapsType-textcapstype-}

Gets and sets the text caps type.

```javascript
setCapsType(value: TextCapsType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextCapsType](../textcapstype/) | The value to set. |

### getStrikeType() {#getStrikeType--}

Gets the strike type of the text.

```javascript
getStrikeType() : TextStrikeType;
```


**Returns**

[TextStrikeType](../textstriketype/)

### setStrikeType(TextStrikeType) {#setStrikeType-textstriketype-}

Gets the strike type of the text.

```javascript
setStrikeType(value: TextStrikeType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextStrikeType](../textstriketype/) | The value to set. |

### isStrikeout() {#isStrikeout--}

Gets or sets a value indicating whether the font is single strikeout.

```javascript
isStrikeout() : boolean;
```


### setIsStrikeout(boolean) {#setIsStrikeout-boolean-}

Gets or sets a value indicating whether the font is single strikeout.

```javascript
setIsStrikeout(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getScriptOffset() {#getScriptOffset--}

Gets and sets the script offset,in unit of percentage

```javascript
getScriptOffset() : number;
```


### setScriptOffset(number) {#setScriptOffset-number-}

Gets and sets the script offset,in unit of percentage

```javascript
setScriptOffset(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### isSuperscript() {#isSuperscript--}

Gets or sets a value indicating whether the font is super script.

```javascript
isSuperscript() : boolean;
```


### setIsSuperscript(boolean) {#setIsSuperscript-boolean-}

Gets or sets a value indicating whether the font is super script.

```javascript
setIsSuperscript(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isSubscript() {#isSubscript--}

Gets or sets a value indicating whether the font is subscript.

```javascript
isSubscript() : boolean;
```


### setIsSubscript(boolean) {#setIsSubscript-boolean-}

Gets or sets a value indicating whether the font is subscript.

```javascript
setIsSubscript(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getUnderline() {#getUnderline--}

Gets or sets the font underline type.

```javascript
getUnderline() : FontUnderlineType;
```


**Returns**

[FontUnderlineType](../fontunderlinetype/)

### setUnderline(FontUnderlineType) {#setUnderline-fontunderlinetype-}

Gets or sets the font underline type.

```javascript
setUnderline(value: FontUnderlineType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [FontUnderlineType](../fontunderlinetype/) | The value to set. |

### getDoubleSize() {#getDoubleSize--}

Gets and sets the double size of the font.

```javascript
getDoubleSize() : number;
```


### setDoubleSize(number) {#setDoubleSize-number-}

Gets and sets the double size of the font.

```javascript
setDoubleSize(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getSize() {#getSize--}

Gets or sets the size of the font.

```javascript
getSize() : number;
```


### setSize(number) {#setSize-number-}

Gets or sets the size of the font.

```javascript
setSize(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getThemeColor() {#getThemeColor--}

Gets and sets the theme color.

```javascript
getThemeColor() : ThemeColor;
```


**Returns**

[ThemeColor](../themecolor/)

**Remarks**

If the font color is not a theme color, NULL will be returned.

### setThemeColor(ThemeColor) {#setThemeColor-themecolor-}

Gets and sets the theme color.

```javascript
setThemeColor(value: ThemeColor) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ThemeColor](../themecolor/) | The value to set. |

**Remarks**

If the font color is not a theme color, NULL will be returned.

### getColor() {#getColor--}

Gets or sets the [Color](../color/) of the font.

```javascript
getColor() : Color;
```


**Returns**

[Color](../color/)

### setColor(Color) {#setColor-color-}

Gets or sets the [Color](../color/) of the font.

```javascript
setColor(value: Color) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../color/) | The value to set. |

### getArgbColor() {#getArgbColor--}

Gets and sets the color with a 32-bit ARGB value.

```javascript
getArgbColor() : number;
```


### setArgbColor(number) {#setArgbColor-number-}

Gets and sets the color with a 32-bit ARGB value.

```javascript
setArgbColor(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### isNormalizeHeights() {#isNormalizeHeights--}

Indicates whether the normalization of height that is to be applied to the text run.

```javascript
isNormalizeHeights() : boolean;
```


### setIsNormalizeHeights(boolean) {#setIsNormalizeHeights-boolean-}

Indicates whether the normalization of height that is to be applied to the text run.

```javascript
setIsNormalizeHeights(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getSchemeType() {#getSchemeType--}

Gets and sets the scheme type of the font.

```javascript
getSchemeType() : FontSchemeType;
```


**Returns**

[FontSchemeType](../fontschemetype/)

### setSchemeType(FontSchemeType) {#setSchemeType-fontschemetype-}

Gets and sets the scheme type of the font.

```javascript
setSchemeType(value: FontSchemeType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [FontSchemeType](../fontschemetype/) | The value to set. |

### equals(Font) {#equals-font-}

Checks if two fonts are equals.

```javascript
equals(font: Font) : boolean;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| font | [Font](../font/) | Compared font object. |

**Returns**

True if equal to the compared font object.

### toString() {#toString--}

Returns a string represents the current Cell object.

```javascript
toString() : string;
```



