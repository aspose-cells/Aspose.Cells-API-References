##TextParagraph
Represents the text paragraph setting.
## TextParagraph class
Represents the text paragraph setting.
```javascript
class TextParagraph extends FontSetting;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor(FontSetting)](#constructor-fontsetting-)| Constructs from a parent object convertible to this. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [bullet](#bullet--)| Bullet | Readonly. Gets the bullet. |
| [lineSpaceSizeType](#lineSpaceSizeType--)| LineSpaceSizeType | Gets and sets the amount of vertical white space that will be used within a paragraph. |
| [lineSpace](#lineSpace--)| number | Gets and sets the amount of vertical white space that will be used within a paragraph. |
| [spaceAfterSizeType](#spaceAfterSizeType--)| LineSpaceSizeType | Gets and sets the amount of vertical white space that will be present after a paragraph. |
| [spaceAfter](#spaceAfter--)| number | Gets and sets the amount of vertical white space that will be present after a paragraph. |
| [spaceBeforeSizeType](#spaceBeforeSizeType--)| LineSpaceSizeType | Gets and sets the amount of vertical white space that will be present before a paragraph. |
| [spaceBefore](#spaceBefore--)| number | Gets and sets the amount of vertical white space that will be present before a paragraph. |
| [stops](#stops--)| TextTabStopCollection | Readonly. Gets tab stop list. |
| [isLatinLineBreak](#isLatinLineBreak--)| boolean | Specifies whether a Latin word can be broken in half and wrapped onto the next line without a hyphen being added. |
| [isEastAsianLineBreak](#isEastAsianLineBreak--)| boolean | Specifies whether an East Asian word can be broken in half and wrapped onto the next line without a hyphen being added. |
| [isHangingPunctuation](#isHangingPunctuation--)| boolean | Specifies whether punctuation is to be forcefully laid out on a line of text or put on a different line of text. |
| [rightMargin](#rightMargin--)| number | Specifies the right margin of the paragraph. |
| [leftMargin](#leftMargin--)| number | Specifies the left margin of the paragraph. |
| [firstLineIndent](#firstLineIndent--)| number | Specifies the indent size that will be applied to the first line of text in the paragraph. |
| [fontAlignType](#fontAlignType--)| TextFontAlignType | Determines where vertically on a line of text the actual words are positioned. This deals with vertical placement of the characters with respect to the baselines. |
| [alignmentType](#alignmentType--)| TextAlignmentType | Gets and sets the text horizontal alignment type of the paragraph. |
| [defaultTabSize](#defaultTabSize--)| number | Gets and sets the default size for a tab character within this paragraph. |
| [children](#children--)| FontSetting[] | Readonly. Gets all text runs in this paragraph. If this paragraph is empty, return paragraph itself. |
| [startIndex](#startIndex--)| number | Readonly. Gets the start index of the characters. |
| [length](#length--)| number | Readonly. Gets the length of the characters. |
| [font](#font--)| Font | Readonly. Returns the font of this object. |
| [textOptions](#textOptions--)| TextOptions | Readonly. Returns the text options. |
## Methods
| Method | Description |
| --- | --- |
| [getBullet()](#getBullet--)| <b>@deprecated.</b> Please use the 'bullet' property instead. Gets the bullet. |
| [getLineSpaceSizeType()](#getLineSpaceSizeType--)| <b>@deprecated.</b> Please use the 'lineSpaceSizeType' property instead. Gets and sets the amount of vertical white space that will be used within a paragraph. |
| [setLineSpaceSizeType(LineSpaceSizeType)](#setLineSpaceSizeType-linespacesizetype-)| <b>@deprecated.</b> Please use the 'lineSpaceSizeType' property instead. Gets and sets the amount of vertical white space that will be used within a paragraph. |
| [getLineSpace()](#getLineSpace--)| <b>@deprecated.</b> Please use the 'lineSpace' property instead. Gets and sets the amount of vertical white space that will be used within a paragraph. |
| [setLineSpace(number)](#setLineSpace-number-)| <b>@deprecated.</b> Please use the 'lineSpace' property instead. Gets and sets the amount of vertical white space that will be used within a paragraph. |
| [getSpaceAfterSizeType()](#getSpaceAfterSizeType--)| <b>@deprecated.</b> Please use the 'spaceAfterSizeType' property instead. Gets and sets the amount of vertical white space that will be present after a paragraph. |
| [setSpaceAfterSizeType(LineSpaceSizeType)](#setSpaceAfterSizeType-linespacesizetype-)| <b>@deprecated.</b> Please use the 'spaceAfterSizeType' property instead. Gets and sets the amount of vertical white space that will be present after a paragraph. |
| [getSpaceAfter()](#getSpaceAfter--)| <b>@deprecated.</b> Please use the 'spaceAfter' property instead. Gets and sets the amount of vertical white space that will be present after a paragraph. |
| [setSpaceAfter(number)](#setSpaceAfter-number-)| <b>@deprecated.</b> Please use the 'spaceAfter' property instead. Gets and sets the amount of vertical white space that will be present after a paragraph. |
| [getSpaceBeforeSizeType()](#getSpaceBeforeSizeType--)| <b>@deprecated.</b> Please use the 'spaceBeforeSizeType' property instead. Gets and sets the amount of vertical white space that will be present before a paragraph. |
| [setSpaceBeforeSizeType(LineSpaceSizeType)](#setSpaceBeforeSizeType-linespacesizetype-)| <b>@deprecated.</b> Please use the 'spaceBeforeSizeType' property instead. Gets and sets the amount of vertical white space that will be present before a paragraph. |
| [getSpaceBefore()](#getSpaceBefore--)| <b>@deprecated.</b> Please use the 'spaceBefore' property instead. Gets and sets the amount of vertical white space that will be present before a paragraph. |
| [setSpaceBefore(number)](#setSpaceBefore-number-)| <b>@deprecated.</b> Please use the 'spaceBefore' property instead. Gets and sets the amount of vertical white space that will be present before a paragraph. |
| [getStops()](#getStops--)| <b>@deprecated.</b> Please use the 'stops' property instead. Gets tab stop list. |
| [isLatinLineBreak()](#isLatinLineBreak--)| <b>@deprecated.</b> Please use the 'isLatinLineBreak' property instead. Specifies whether a Latin word can be broken in half and wrapped onto the next line without a hyphen being added. |
| [setIsLatinLineBreak(boolean)](#setIsLatinLineBreak-boolean-)| <b>@deprecated.</b> Please use the 'isLatinLineBreak' property instead. Specifies whether a Latin word can be broken in half and wrapped onto the next line without a hyphen being added. |
| [isEastAsianLineBreak()](#isEastAsianLineBreak--)| <b>@deprecated.</b> Please use the 'isEastAsianLineBreak' property instead. Specifies whether an East Asian word can be broken in half and wrapped onto the next line without a hyphen being added. |
| [setIsEastAsianLineBreak(boolean)](#setIsEastAsianLineBreak-boolean-)| <b>@deprecated.</b> Please use the 'isEastAsianLineBreak' property instead. Specifies whether an East Asian word can be broken in half and wrapped onto the next line without a hyphen being added. |
| [isHangingPunctuation()](#isHangingPunctuation--)| <b>@deprecated.</b> Please use the 'isHangingPunctuation' property instead. Specifies whether punctuation is to be forcefully laid out on a line of text or put on a different line of text. |
| [setIsHangingPunctuation(boolean)](#setIsHangingPunctuation-boolean-)| <b>@deprecated.</b> Please use the 'isHangingPunctuation' property instead. Specifies whether punctuation is to be forcefully laid out on a line of text or put on a different line of text. |
| [getRightMargin()](#getRightMargin--)| <b>@deprecated.</b> Please use the 'rightMargin' property instead. Specifies the right margin of the paragraph. |
| [setRightMargin(number)](#setRightMargin-number-)| <b>@deprecated.</b> Please use the 'rightMargin' property instead. Specifies the right margin of the paragraph. |
| [getLeftMargin()](#getLeftMargin--)| <b>@deprecated.</b> Please use the 'leftMargin' property instead. Specifies the left margin of the paragraph. |
| [setLeftMargin(number)](#setLeftMargin-number-)| <b>@deprecated.</b> Please use the 'leftMargin' property instead. Specifies the left margin of the paragraph. |
| [getFirstLineIndent()](#getFirstLineIndent--)| <b>@deprecated.</b> Please use the 'firstLineIndent' property instead. Specifies the indent size that will be applied to the first line of text in the paragraph. |
| [setFirstLineIndent(number)](#setFirstLineIndent-number-)| <b>@deprecated.</b> Please use the 'firstLineIndent' property instead. Specifies the indent size that will be applied to the first line of text in the paragraph. |
| [getFontAlignType()](#getFontAlignType--)| <b>@deprecated.</b> Please use the 'fontAlignType' property instead. Determines where vertically on a line of text the actual words are positioned. This deals with vertical placement of the characters with respect to the baselines. |
| [setFontAlignType(TextFontAlignType)](#setFontAlignType-textfontaligntype-)| <b>@deprecated.</b> Please use the 'fontAlignType' property instead. Determines where vertically on a line of text the actual words are positioned. This deals with vertical placement of the characters with respect to the baselines. |
| [getAlignmentType()](#getAlignmentType--)| <b>@deprecated.</b> Please use the 'alignmentType' property instead. Gets and sets the text horizontal alignment type of the paragraph. |
| [setAlignmentType(TextAlignmentType)](#setAlignmentType-textalignmenttype-)| <b>@deprecated.</b> Please use the 'alignmentType' property instead. Gets and sets the text horizontal alignment type of the paragraph. |
| [getDefaultTabSize()](#getDefaultTabSize--)| <b>@deprecated.</b> Please use the 'defaultTabSize' property instead. Gets and sets the default size for a tab character within this paragraph. |
| [setDefaultTabSize(number)](#setDefaultTabSize-number-)| <b>@deprecated.</b> Please use the 'defaultTabSize' property instead. Gets and sets the default size for a tab character within this paragraph. |
| [getChildren()](#getChildren--)| <b>@deprecated.</b> Please use the 'children' property instead. Gets all text runs in this paragraph. If this paragraph is empty, return paragraph itself. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [getStartIndex()](#getStartIndex--)| <b>@deprecated.</b> Please use the 'startIndex' property instead. Gets the start index of the characters. |
| [getLength()](#getLength--)| <b>@deprecated.</b> Please use the 'length' property instead. Gets the length of the characters. |
| [getFont()](#getFont--)| <b>@deprecated.</b> Please use the 'font' property instead. Returns the font of this object. |
| [getTextOptions()](#getTextOptions--)| <b>@deprecated.</b> Please use the 'textOptions' property instead. Returns the text options. |
| [setWordArtStyle(PresetWordArtStyle)](#setWordArtStyle-presetwordartstyle-)| Sets the preset WordArt style. |
| [getType()](#getType--)| Gets the type of text node. |
### constructor(FontSetting) {#constructor-fontsetting-}
Constructs from a parent object convertible to this.
```javascript
constructor(obj: FontSetting);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | FontSetting | The parent object. |
### bullet {#bullet--}
Readonly. Gets the bullet.
```javascript
bullet : Bullet;
```
### lineSpaceSizeType {#lineSpaceSizeType--}
Gets and sets the amount of vertical white space that will be used within a paragraph.
```javascript
lineSpaceSizeType : LineSpaceSizeType;
```
### lineSpace {#lineSpace--}
Gets and sets the amount of vertical white space that will be used within a paragraph.
```javascript
lineSpace : number;
```
### spaceAfterSizeType {#spaceAfterSizeType--}
Gets and sets the amount of vertical white space that will be present after a paragraph.
```javascript
spaceAfterSizeType : LineSpaceSizeType;
```
### spaceAfter {#spaceAfter--}
Gets and sets the amount of vertical white space that will be present after a paragraph.
```javascript
spaceAfter : number;
```
### spaceBeforeSizeType {#spaceBeforeSizeType--}
Gets and sets the amount of vertical white space that will be present before a paragraph.
```javascript
spaceBeforeSizeType : LineSpaceSizeType;
```
### spaceBefore {#spaceBefore--}
Gets and sets the amount of vertical white space that will be present before a paragraph.
```javascript
spaceBefore : number;
```
### stops {#stops--}
Readonly. Gets tab stop list.
```javascript
stops : TextTabStopCollection;
```
### isLatinLineBreak {#isLatinLineBreak--}
Specifies whether a Latin word can be broken in half and wrapped onto the next line without a hyphen being added.
```javascript
isLatinLineBreak : boolean;
```
### isEastAsianLineBreak {#isEastAsianLineBreak--}
Specifies whether an East Asian word can be broken in half and wrapped onto the next line without a hyphen being added.
```javascript
isEastAsianLineBreak : boolean;
```
### isHangingPunctuation {#isHangingPunctuation--}
Specifies whether punctuation is to be forcefully laid out on a line of text or put on a different line of text.
```javascript
isHangingPunctuation : boolean;
```
### rightMargin {#rightMargin--}
Specifies the right margin of the paragraph.
```javascript
rightMargin : number;
```
### leftMargin {#leftMargin--}
Specifies the left margin of the paragraph.
```javascript
leftMargin : number;
```
### firstLineIndent {#firstLineIndent--}
Specifies the indent size that will be applied to the first line of text in the paragraph.
```javascript
firstLineIndent : number;
```
### fontAlignType {#fontAlignType--}
Determines where vertically on a line of text the actual words are positioned. This deals with vertical placement of the characters with respect to the baselines.
```javascript
fontAlignType : TextFontAlignType;
```
### alignmentType {#alignmentType--}
Gets and sets the text horizontal alignment type of the paragraph.
```javascript
alignmentType : TextAlignmentType;
```
### defaultTabSize {#defaultTabSize--}
Gets and sets the default size for a tab character within this paragraph.
```javascript
defaultTabSize : number;
```
### children {#children--}
Readonly. Gets all text runs in this paragraph. If this paragraph is empty, return paragraph itself.
```javascript
children : FontSetting[];
```
### startIndex {#startIndex--}
Readonly. Gets the start index of the characters.
```javascript
startIndex : number;
```
### length {#length--}
Readonly. Gets the length of the characters.
```javascript
length : number;
```
### font {#font--}
Readonly. Returns the font of this object.
```javascript
font : Font;
```
### textOptions {#textOptions--}
Readonly. Returns the text options.
```javascript
textOptions : TextOptions;
```
### getBullet() {#getBullet--}
```javascript
getBullet() : Bullet;
```
**Returns**
[Bullet](../bullet/)
### getLineSpaceSizeType() {#getLineSpaceSizeType--}
```javascript
getLineSpaceSizeType() : LineSpaceSizeType;
```
**Returns**
[LineSpaceSizeType](../linespacesizetype/)
### setLineSpaceSizeType(LineSpaceSizeType) {#setLineSpaceSizeType-linespacesizetype-}
```javascript
setLineSpaceSizeType(value: LineSpaceSizeType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [LineSpaceSizeType](../linespacesizetype/) | The value to set. |
### getLineSpace() {#getLineSpace--}
```javascript
getLineSpace() : number;
```
### setLineSpace(number) {#setLineSpace-number-}
```javascript
setLineSpace(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getSpaceAfterSizeType() {#getSpaceAfterSizeType--}
```javascript
getSpaceAfterSizeType() : LineSpaceSizeType;
```
**Returns**
[LineSpaceSizeType](../linespacesizetype/)
### setSpaceAfterSizeType(LineSpaceSizeType) {#setSpaceAfterSizeType-linespacesizetype-}
```javascript
setSpaceAfterSizeType(value: LineSpaceSizeType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [LineSpaceSizeType](../linespacesizetype/) | The value to set. |
### getSpaceAfter() {#getSpaceAfter--}
```javascript
getSpaceAfter() : number;
```
### setSpaceAfter(number) {#setSpaceAfter-number-}
```javascript
setSpaceAfter(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getSpaceBeforeSizeType() {#getSpaceBeforeSizeType--}
```javascript
getSpaceBeforeSizeType() : LineSpaceSizeType;
```
**Returns**
[LineSpaceSizeType](../linespacesizetype/)
### setSpaceBeforeSizeType(LineSpaceSizeType) {#setSpaceBeforeSizeType-linespacesizetype-}
```javascript
setSpaceBeforeSizeType(value: LineSpaceSizeType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [LineSpaceSizeType](../linespacesizetype/) | The value to set. |
### getSpaceBefore() {#getSpaceBefore--}
```javascript
getSpaceBefore() : number;
```
### setSpaceBefore(number) {#setSpaceBefore-number-}
```javascript
setSpaceBefore(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getStops() {#getStops--}
```javascript
getStops() : TextTabStopCollection;
```
**Returns**
[TextTabStopCollection](../texttabstopcollection/)
### isLatinLineBreak() {#isLatinLineBreak--}
```javascript
isLatinLineBreak() : boolean;
```
### setIsLatinLineBreak(boolean) {#setIsLatinLineBreak-boolean-}
```javascript
setIsLatinLineBreak(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### isEastAsianLineBreak() {#isEastAsianLineBreak--}
```javascript
isEastAsianLineBreak() : boolean;
```
### setIsEastAsianLineBreak(boolean) {#setIsEastAsianLineBreak-boolean-}
```javascript
setIsEastAsianLineBreak(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### isHangingPunctuation() {#isHangingPunctuation--}
```javascript
isHangingPunctuation() : boolean;
```
### setIsHangingPunctuation(boolean) {#setIsHangingPunctuation-boolean-}
```javascript
setIsHangingPunctuation(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getRightMargin() {#getRightMargin--}
```javascript
getRightMargin() : number;
```
### setRightMargin(number) {#setRightMargin-number-}
```javascript
setRightMargin(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getLeftMargin() {#getLeftMargin--}
```javascript
getLeftMargin() : number;
```
### setLeftMargin(number) {#setLeftMargin-number-}
```javascript
setLeftMargin(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getFirstLineIndent() {#getFirstLineIndent--}
```javascript
getFirstLineIndent() : number;
```
### setFirstLineIndent(number) {#setFirstLineIndent-number-}
```javascript
setFirstLineIndent(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getFontAlignType() {#getFontAlignType--}
```javascript
getFontAlignType() : TextFontAlignType;
```
**Returns**
[TextFontAlignType](../textfontaligntype/)
### setFontAlignType(TextFontAlignType) {#setFontAlignType-textfontaligntype-}
```javascript
setFontAlignType(value: TextFontAlignType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextFontAlignType](../textfontaligntype/) | The value to set. |
### getAlignmentType() {#getAlignmentType--}
```javascript
getAlignmentType() : TextAlignmentType;
```
**Returns**
[TextAlignmentType](../textalignmenttype/)
### setAlignmentType(TextAlignmentType) {#setAlignmentType-textalignmenttype-}
```javascript
setAlignmentType(value: TextAlignmentType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextAlignmentType](../textalignmenttype/) | The value to set. |
### getDefaultTabSize() {#getDefaultTabSize--}
```javascript
getDefaultTabSize() : number;
```
### setDefaultTabSize(number) {#setDefaultTabSize-number-}
```javascript
setDefaultTabSize(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getChildren() {#getChildren--}
```javascript
getChildren() : FontSetting[];
```
**Returns**
[FontSetting](../fontsetting/)[]
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
### getStartIndex() {#getStartIndex--}
```javascript
getStartIndex() : number;
```
### getLength() {#getLength--}
```javascript
getLength() : number;
```
### getFont() {#getFont--}
```javascript
getFont() : Font;
```
**Returns**
[Font](../font/)
### getTextOptions() {#getTextOptions--}
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
