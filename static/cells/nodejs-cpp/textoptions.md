##TextOptions
Represents the text options.
## TextOptions class
Represents the text options.
```javascript
class TextOptions extends Font;
```
## Constructors
| Constructor | Description |
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
| [charset](#charset--)| number | Represent the character set. |
| [isItalic](#isItalic--)| boolean | Gets or sets a value indicating whether the font is italic. |
| [isBold](#isBold--)| boolean | Gets or sets a value indicating whether the font is bold. |
| [capsType](#capsType--)| TextCapsType | Gets and sets the text caps type. |
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
| [isNormalizeHeights](#isNormalizeHeights--)| boolean | Indicates whether the normalization of height that is to be applied to the text run. |
| [schemeType](#schemeType--)| FontSchemeType | Gets and sets the scheme type of the font. |
## Methods
| Method | Description |
| --- | --- |
| [getLanguageCode()](#getLanguageCode--)| <b>@deprecated.</b> Please use the 'languageCode' property instead. Gets and sets the user interface language. |
| [setLanguageCode(CountryCode)](#setLanguageCode-countrycode-)| <b>@deprecated.</b> Please use the 'languageCode' property instead. Gets and sets the user interface language. |
| [getLatinName()](#getLatinName--)| <b>@deprecated.</b> Please use the 'latinName' property instead. Gets and sets the latin name. |
| [setLatinName(string)](#setLatinName-string-)| <b>@deprecated.</b> Please use the 'latinName' property instead. Gets and sets the latin name. |
| [getFarEastName()](#getFarEastName--)| <b>@deprecated.</b> Please use the 'farEastName' property instead. Gets and sets the FarEast name. |
| [setFarEastName(string)](#setFarEastName-string-)| <b>@deprecated.</b> Please use the 'farEastName' property instead. Gets and sets the FarEast name. |
| [getFill()](#getFill--)| <b>@deprecated.</b> Please use the 'fill' property instead. Represents the fill format of the text. |
| [getOutline()](#getOutline--)| <b>@deprecated.</b> Please use the 'outline' property instead. Represents the outline format of the text. |
| [getShadow()](#getShadow--)| <b>@deprecated.</b> Please use the 'shadow' property instead. Represents a [ShadowEffect](../shadoweffect/) object that specifies shadow effect for the chart element or shape. |
| [getUnderlineColor()](#getUnderlineColor--)| <b>@deprecated.</b> Please use the 'underlineColor' property instead. Gets or sets the color of underline. |
| [setUnderlineColor(CellsColor)](#setUnderlineColor-cellscolor-)| <b>@deprecated.</b> Please use the 'underlineColor' property instead. Gets or sets the color of underline. |
| [getKerning()](#getKerning--)| <b>@deprecated.</b> Please use the 'kerning' property instead. Specifies the minimum font size at which character kerning will occur for this text run. |
| [setKerning(number)](#setKerning-number-)| <b>@deprecated.</b> Please use the 'kerning' property instead. Specifies the minimum font size at which character kerning will occur for this text run. |
| [getSpacing()](#getSpacing--)| <b>@deprecated.</b> Please use the 'spacing' property instead. Specifies the spacing between characters within a text run. |
| [setSpacing(number)](#setSpacing-number-)| <b>@deprecated.</b> Please use the 'spacing' property instead. Specifies the spacing between characters within a text run. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [getCharset()](#getCharset--)| <b>@deprecated.</b> Please use the 'charset' property instead. Represent the character set. |
| [setCharset(number)](#setCharset-number-)| <b>@deprecated.</b> Please use the 'charset' property instead. Represent the character set. |
| [isItalic()](#isItalic--)| <b>@deprecated.</b> Please use the 'isItalic' property instead. Gets or sets a value indicating whether the font is italic. |
| [setIsItalic(boolean)](#setIsItalic-boolean-)| <b>@deprecated.</b> Please use the 'isItalic' property instead. Gets or sets a value indicating whether the font is italic. |
| [isBold()](#isBold--)| <b>@deprecated.</b> Please use the 'isBold' property instead. Gets or sets a value indicating whether the font is bold. |
| [setIsBold(boolean)](#setIsBold-boolean-)| <b>@deprecated.</b> Please use the 'isBold' property instead. Gets or sets a value indicating whether the font is bold. |
| [getCapsType()](#getCapsType--)| <b>@deprecated.</b> Please use the 'capsType' property instead. Gets and sets the text caps type. |
| [setCapsType(TextCapsType)](#setCapsType-textcapstype-)| <b>@deprecated.</b> Please use the 'capsType' property instead. Gets and sets the text caps type. |
| [getStrikeType()](#getStrikeType--)| <b>@deprecated.</b> Please use the 'strikeType' property instead. Gets the strike type of the text. |
| [setStrikeType(TextStrikeType)](#setStrikeType-textstriketype-)| <b>@deprecated.</b> Please use the 'strikeType' property instead. Gets the strike type of the text. |
| [isStrikeout()](#isStrikeout--)| <b>@deprecated.</b> Please use the 'isStrikeout' property instead. Gets or sets a value indicating whether the font is single strikeout. |
| [setIsStrikeout(boolean)](#setIsStrikeout-boolean-)| <b>@deprecated.</b> Please use the 'isStrikeout' property instead. Gets or sets a value indicating whether the font is single strikeout. |
| [getScriptOffset()](#getScriptOffset--)| <b>@deprecated.</b> Please use the 'scriptOffset' property instead. Gets and sets the script offset,in unit of percentage |
| [setScriptOffset(number)](#setScriptOffset-number-)| <b>@deprecated.</b> Please use the 'scriptOffset' property instead. Gets and sets the script offset,in unit of percentage |
| [isSuperscript()](#isSuperscript--)| <b>@deprecated.</b> Please use the 'isSuperscript' property instead. Gets or sets a value indicating whether the font is super script. |
| [setIsSuperscript(boolean)](#setIsSuperscript-boolean-)| <b>@deprecated.</b> Please use the 'isSuperscript' property instead. Gets or sets a value indicating whether the font is super script. |
| [isSubscript()](#isSubscript--)| <b>@deprecated.</b> Please use the 'isSubscript' property instead. Gets or sets a value indicating whether the font is subscript. |
| [setIsSubscript(boolean)](#setIsSubscript-boolean-)| <b>@deprecated.</b> Please use the 'isSubscript' property instead. Gets or sets a value indicating whether the font is subscript. |
| [getUnderline()](#getUnderline--)| <b>@deprecated.</b> Please use the 'underline' property instead. Gets or sets the font underline type. |
| [setUnderline(FontUnderlineType)](#setUnderline-fontunderlinetype-)| <b>@deprecated.</b> Please use the 'underline' property instead. Gets or sets the font underline type. |
| [getDoubleSize()](#getDoubleSize--)| <b>@deprecated.</b> Please use the 'doubleSize' property instead. Gets and sets the double size of the font. |
| [setDoubleSize(number)](#setDoubleSize-number-)| <b>@deprecated.</b> Please use the 'doubleSize' property instead. Gets and sets the double size of the font. |
| [getSize()](#getSize--)| <b>@deprecated.</b> Please use the 'size' property instead. Gets or sets the size of the font. |
| [setSize(number)](#setSize-number-)| <b>@deprecated.</b> Please use the 'size' property instead. Gets or sets the size of the font. |
| [getThemeColor()](#getThemeColor--)| <b>@deprecated.</b> Please use the 'themeColor' property instead. Gets and sets the theme color. |
| [setThemeColor(ThemeColor)](#setThemeColor-themecolor-)| <b>@deprecated.</b> Please use the 'themeColor' property instead. Gets and sets the theme color. |
| [getColor()](#getColor--)| <b>@deprecated.</b> Please use the 'color' property instead. Gets or sets the [Color](../color/) of the font. |
| [setColor(Color)](#setColor-color-)| <b>@deprecated.</b> Please use the 'color' property instead. Gets or sets the [Color](../color/) of the font. |
| [getArgbColor()](#getArgbColor--)| <b>@deprecated.</b> Please use the 'argbColor' property instead. Gets and sets the color with a 32-bit ARGB value. |
| [setArgbColor(number)](#setArgbColor-number-)| <b>@deprecated.</b> Please use the 'argbColor' property instead. Gets and sets the color with a 32-bit ARGB value. |
| [isNormalizeHeights()](#isNormalizeHeights--)| <b>@deprecated.</b> Please use the 'isNormalizeHeights' property instead. Indicates whether the normalization of height that is to be applied to the text run. |
| [setIsNormalizeHeights(boolean)](#setIsNormalizeHeights-boolean-)| <b>@deprecated.</b> Please use the 'isNormalizeHeights' property instead. Indicates whether the normalization of height that is to be applied to the text run. |
| [getSchemeType()](#getSchemeType--)| <b>@deprecated.</b> Please use the 'schemeType' property instead. Gets and sets the scheme type of the font. |
| [setSchemeType(FontSchemeType)](#setSchemeType-fontschemetype-)| <b>@deprecated.</b> Please use the 'schemeType' property instead. Gets and sets the scheme type of the font. |
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
### capsType {#capsType--}
Gets and sets the text caps type.
```javascript
capsType : TextCapsType;
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
### isNormalizeHeights {#isNormalizeHeights--}
Indicates whether the normalization of height that is to be applied to the text run.
```javascript
isNormalizeHeights : boolean;
```
### schemeType {#schemeType--}
Gets and sets the scheme type of the font.
```javascript
schemeType : FontSchemeType;
```
### getLanguageCode() {#getLanguageCode--}
```javascript
getLanguageCode() : CountryCode;
```
**Returns**
[CountryCode](../countrycode/)
### setLanguageCode(CountryCode) {#setLanguageCode-countrycode-}
```javascript
setLanguageCode(value: CountryCode) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CountryCode](../countrycode/) | The value to set. |
### getLatinName() {#getLatinName--}
```javascript
getLatinName() : string;
```
### setLatinName(string) {#setLatinName-string-}
```javascript
setLatinName(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getFarEastName() {#getFarEastName--}
```javascript
getFarEastName() : string;
```
### setFarEastName(string) {#setFarEastName-string-}
```javascript
setFarEastName(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getFill() {#getFill--}
```javascript
getFill() : FillFormat;
```
**Returns**
[FillFormat](../fillformat/)
### getOutline() {#getOutline--}
```javascript
getOutline() : LineFormat;
```
**Returns**
[LineFormat](../lineformat/)
### getShadow() {#getShadow--}
```javascript
getShadow() : ShadowEffect;
```
**Returns**
[ShadowEffect](../shadoweffect/)
### getUnderlineColor() {#getUnderlineColor--}
```javascript
getUnderlineColor() : CellsColor;
```
**Returns**
[CellsColor](../cellscolor/)
### setUnderlineColor(CellsColor) {#setUnderlineColor-cellscolor-}
```javascript
setUnderlineColor(value: CellsColor) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CellsColor](../cellscolor/) | The value to set. |
### getKerning() {#getKerning--}
```javascript
getKerning() : number;
```
### setKerning(number) {#setKerning-number-}
```javascript
setKerning(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getSpacing() {#getSpacing--}
```javascript
getSpacing() : number;
```
### setSpacing(number) {#setSpacing-number-}
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
```javascript
getCharset() : number;
```
### setCharset(number) {#setCharset-number-}
```javascript
setCharset(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### isItalic() {#isItalic--}
```javascript
isItalic() : boolean;
```
### setIsItalic(boolean) {#setIsItalic-boolean-}
```javascript
setIsItalic(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### isBold() {#isBold--}
```javascript
isBold() : boolean;
```
### setIsBold(boolean) {#setIsBold-boolean-}
```javascript
setIsBold(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getCapsType() {#getCapsType--}
```javascript
getCapsType() : TextCapsType;
```
**Returns**
[TextCapsType](../textcapstype/)
### setCapsType(TextCapsType) {#setCapsType-textcapstype-}
```javascript
setCapsType(value: TextCapsType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextCapsType](../textcapstype/) | The value to set. |
### getStrikeType() {#getStrikeType--}
```javascript
getStrikeType() : TextStrikeType;
```
**Returns**
[TextStrikeType](../textstriketype/)
### setStrikeType(TextStrikeType) {#setStrikeType-textstriketype-}
```javascript
setStrikeType(value: TextStrikeType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextStrikeType](../textstriketype/) | The value to set. |
### isStrikeout() {#isStrikeout--}
```javascript
isStrikeout() : boolean;
```
### setIsStrikeout(boolean) {#setIsStrikeout-boolean-}
```javascript
setIsStrikeout(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getScriptOffset() {#getScriptOffset--}
```javascript
getScriptOffset() : number;
```
### setScriptOffset(number) {#setScriptOffset-number-}
```javascript
setScriptOffset(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### isSuperscript() {#isSuperscript--}
```javascript
isSuperscript() : boolean;
```
### setIsSuperscript(boolean) {#setIsSuperscript-boolean-}
```javascript
setIsSuperscript(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### isSubscript() {#isSubscript--}
```javascript
isSubscript() : boolean;
```
### setIsSubscript(boolean) {#setIsSubscript-boolean-}
```javascript
setIsSubscript(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getUnderline() {#getUnderline--}
```javascript
getUnderline() : FontUnderlineType;
```
**Returns**
[FontUnderlineType](../fontunderlinetype/)
### setUnderline(FontUnderlineType) {#setUnderline-fontunderlinetype-}
```javascript
setUnderline(value: FontUnderlineType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [FontUnderlineType](../fontunderlinetype/) | The value to set. |
### getDoubleSize() {#getDoubleSize--}
```javascript
getDoubleSize() : number;
```
### setDoubleSize(number) {#setDoubleSize-number-}
```javascript
setDoubleSize(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getSize() {#getSize--}
```javascript
getSize() : number;
```
### setSize(number) {#setSize-number-}
```javascript
setSize(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getThemeColor() {#getThemeColor--}
```javascript
getThemeColor() : ThemeColor;
```
**Returns**
[ThemeColor](../themecolor/)
**Remarks**
If the font color is not a theme color, NULL will be returned.
### setThemeColor(ThemeColor) {#setThemeColor-themecolor-}
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
```javascript
getColor() : Color;
```
**Returns**
[Color](../color/)
### setColor(Color) {#setColor-color-}
```javascript
setColor(value: Color) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../color/) | The value to set. |
### getArgbColor() {#getArgbColor--}
```javascript
getArgbColor() : number;
```
### setArgbColor(number) {#setArgbColor-number-}
```javascript
setArgbColor(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### isNormalizeHeights() {#isNormalizeHeights--}
```javascript
isNormalizeHeights() : boolean;
```
### setIsNormalizeHeights(boolean) {#setIsNormalizeHeights-boolean-}
```javascript
setIsNormalizeHeights(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getSchemeType() {#getSchemeType--}
```javascript
getSchemeType() : FontSchemeType;
```
**Returns**
[FontSchemeType](../fontschemetype/)
### setSchemeType(FontSchemeType) {#setSchemeType-fontschemetype-}
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
