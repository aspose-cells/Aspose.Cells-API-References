##TextParagraph
Represents the text paragraph setting.
## TextParagraph class
Represents the text paragraph setting.
```javascript
class TextParagraph extends FontSetting;
```
## Constructors
| Name | Description |
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
