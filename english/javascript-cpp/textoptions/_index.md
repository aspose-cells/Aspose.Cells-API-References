---
title: TextOptions
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Represents the text options.
type: docs
url: /javascript-cpp/textoptions/
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

## Properties

| Property | Type | Description |
| --- | --- | --- |
| [languageCode](#languageCode--)| CountryCode | Gets and sets the user interface language. |
| [latinName](#latinName--)| string | Gets and sets the latin name. |
| [farEastName](#farEastName--)| string | Gets and sets the FarEast name. |
| [fill](#fill--)| FillFormat | Readonly. Represents the fill format of the text. |
| [outline](#outline--)| LineFormat | Readonly. Represents the outline format of the text. |
| [shadow](#shadow--)| ShadowEffect | Readonly. Represents a [ShadowEffect](../shadoweffect/) object that specifies shadow effect for the chart element or shape. |
| [underlineColor](#underlineColor--)| CellsColor | Gets or sets the color of underline. |
| [kerning](#kerning--)| number | Specifies the minimum font size at which character kerning will occur for this text run. |
| [spacing](#spacing--)| number | Specifies the spacing between characters within a text run. |
| [isNormalizeHeights](#isNormalizeHeights--)| boolean | Indicates whether the normalization of height that is to be applied to the text run. |
| [capsType](#capsType--)| TextCapsType | Gets and sets the text caps type. |
| [charset](#charset--)| number | Represent the character set. |
| [isItalic](#isItalic--)| boolean | Gets or sets a value indicating whether the font is italic. |
| [isBold](#isBold--)| boolean | Gets or sets a value indicating whether the font is bold. |
| [strikeType](#strikeType--)| TextStrikeType | Gets the strike type of the text. |
| [isStrikeout](#isStrikeout--)| boolean | Gets or sets a value indicating whether the font is single strikeout. |
| [scriptOffset](#scriptOffset--)| number | Gets and sets the script offset,in unit of percentage |
| [isSuperscript](#isSuperscript--)| boolean | Gets or sets a value indicating whether the font is super script. |
| [isSubscript](#isSubscript--)| boolean | Gets or sets a value indicating whether the font is subscript. |
| [underline](#underline--)| FontUnderlineType | Gets or sets the font underline type. |
| [doubleSize](#doubleSize--)| number | Gets and sets the double size of the font. |
| [size](#size--)| number | Gets or sets the size of the font. |
| [themeColor](#themeColor--)| ThemeColor | Gets and sets the theme color. |
| [color](#color--)| Color | Gets or sets the [Color](../color/) of the font. |
| [argbColor](#argbColor--)| number | Gets and sets the color with a 32-bit ARGB value. |
| [schemeType](#schemeType--)| FontSchemeType | Gets and sets the scheme type of the font. |

## Methods

| Method | Description |
| --- | --- |
| [equals(Font)](#equals-font-)| Checks if two fonts are equals. |
| [getName()](#getName--)| Gets and sets the name of the shape. |
| [setName(string)](#setName-string-)| Gets and sets the name of the shape. |
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

### languageCode {#languageCode--}

Gets and sets the user interface language.

```javascript
languageCode : CountryCode;
```


### latinName {#latinName--}

Gets and sets the latin name.

```javascript
latinName : string;
```


### farEastName {#farEastName--}

Gets and sets the FarEast name.

```javascript
farEastName : string;
```


### fill {#fill--}

Readonly. Represents the fill format of the text.

```javascript
fill : FillFormat;
```


### outline {#outline--}

Readonly. Represents the outline format of the text.

```javascript
outline : LineFormat;
```


### shadow {#shadow--}

Readonly. Represents a [ShadowEffect](../shadoweffect/) object that specifies shadow effect for the chart element or shape.

```javascript
shadow : ShadowEffect;
```


### underlineColor {#underlineColor--}

Gets or sets the color of underline.

```javascript
underlineColor : CellsColor;
```


### kerning {#kerning--}

Specifies the minimum font size at which character kerning will occur for this text run.

```javascript
kerning : number;
```


### spacing {#spacing--}

Specifies the spacing between characters within a text run.

```javascript
spacing : number;
```


### isNormalizeHeights {#isNormalizeHeights--}

Indicates whether the normalization of height that is to be applied to the text run.

```javascript
isNormalizeHeights : boolean;
```


**Remarks**

Only for the fonts of Shapes or Charts.

### capsType {#capsType--}

Gets and sets the text caps type.

```javascript
capsType : TextCapsType;
```


### charset {#charset--}

Represent the character set.

```javascript
charset : number;
```


### isItalic {#isItalic--}

Gets or sets a value indicating whether the font is italic.

```javascript
isItalic : boolean;
```


### isBold {#isBold--}

Gets or sets a value indicating whether the font is bold.

```javascript
isBold : boolean;
```


### strikeType {#strikeType--}

Gets the strike type of the text.

```javascript
strikeType : TextStrikeType;
```


### isStrikeout {#isStrikeout--}

Gets or sets a value indicating whether the font is single strikeout.

```javascript
isStrikeout : boolean;
```


### scriptOffset {#scriptOffset--}

Gets and sets the script offset,in unit of percentage

```javascript
scriptOffset : number;
```


**Remarks**

Only for shapes and charts.

### isSuperscript {#isSuperscript--}

Gets or sets a value indicating whether the font is super script.

```javascript
isSuperscript : boolean;
```


### isSubscript {#isSubscript--}

Gets or sets a value indicating whether the font is subscript.

```javascript
isSubscript : boolean;
```


### underline {#underline--}

Gets or sets the font underline type.

```javascript
underline : FontUnderlineType;
```


### doubleSize {#doubleSize--}

Gets and sets the double size of the font.

```javascript
doubleSize : number;
```


### size {#size--}

Gets or sets the size of the font.

```javascript
size : number;
```


### themeColor {#themeColor--}

Gets and sets the theme color.

```javascript
themeColor : ThemeColor;
```


**Remarks**

If the font color is not a theme color, NULL will be returned.

### color {#color--}

Gets or sets the [Color](../color/) of the font.

```javascript
color : Color;
```


### argbColor {#argbColor--}

Gets and sets the color with a 32-bit ARGB value.

```javascript
argbColor : number;
```


### schemeType {#schemeType--}

Gets and sets the scheme type of the font.

```javascript
schemeType : FontSchemeType;
```


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

### toString() {#toString--}

Returns a string represents the current Cell object.

```javascript
toString() : string;
```



