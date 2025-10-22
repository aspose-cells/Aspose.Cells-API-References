##TextParagraph Class
'TextParagraph class. Encapsulates the object that represents textparagraph in Go.'
## TextParagraph class
Represents the text paragraph setting.
```go
type TextParagraph struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewTextParagraph](./newtextparagraph/) | Constructs from a parent object. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetBullet](./getbullet/) | Gets the bullet. |
|[GetType](./gettype/) | Gets the type of text node. |
|[GetLineSpaceSizeType](./getlinespacesizetype/) | Gets and sets the amount of vertical white space that will be used within a paragraph. |
|[SetLineSpaceSizeType](./setlinespacesizetype/) | Gets and sets the amount of vertical white space that will be used within a paragraph. |
|[GetLineSpace](./getlinespace/) | Gets and sets the amount of vertical white space that will be used within a paragraph. |
|[SetLineSpace](./setlinespace/) | Gets and sets the amount of vertical white space that will be used within a paragraph. |
|[GetSpaceAfterSizeType](./getspaceaftersizetype/) | Gets and sets the amount of vertical white space that will be present after a paragraph. |
|[SetSpaceAfterSizeType](./setspaceaftersizetype/) | Gets and sets the amount of vertical white space that will be present after a paragraph. |
|[GetSpaceAfter](./getspaceafter/) | Gets and sets the amount of vertical white space that will be present after a paragraph. |
|[SetSpaceAfter](./setspaceafter/) | Gets and sets the amount of vertical white space that will be present after a paragraph. |
|[GetSpaceBeforeSizeType](./getspacebeforesizetype/) | Gets and sets the amount of vertical white space that will be present before a paragraph. |
|[SetSpaceBeforeSizeType](./setspacebeforesizetype/) | Gets and sets the amount of vertical white space that will be present before a paragraph. |
|[GetSpaceBefore](./getspacebefore/) | Gets and sets the amount of vertical white space that will be present before a paragraph. |
|[SetSpaceBefore](./setspacebefore/) | Gets and sets the amount of vertical white space that will be present before a paragraph. |
|[GetStops](./getstops/) | Gets tab stop list. |
|[IsLatinLineBreak](./islatinlinebreak/) | Specifies whether a Latin word can be broken in half and wrapped onto the next line without a hyphen being added. |
|[SetIsLatinLineBreak](./setislatinlinebreak/) | Specifies whether a Latin word can be broken in half and wrapped onto the next line without a hyphen being added. |
|[IsEastAsianLineBreak](./iseastasianlinebreak/) | Specifies whether an East Asian word can be broken in half and wrapped onto the next line without a hyphen being added. |
|[SetIsEastAsianLineBreak](./setiseastasianlinebreak/) | Specifies whether an East Asian word can be broken in half and wrapped onto the next line without a hyphen being added. |
|[IsHangingPunctuation](./ishangingpunctuation/) | Specifies whether punctuation is to be forcefully laid out on a line of text or put on a different line of text. |
|[SetIsHangingPunctuation](./setishangingpunctuation/) | Specifies whether punctuation is to be forcefully laid out on a line of text or put on a different line of text. |
|[GetRightMargin](./getrightmargin/) | Specifies the right margin of the paragraph. |
|[SetRightMargin](./setrightmargin/) | Specifies the right margin of the paragraph. |
|[GetLeftMargin](./getleftmargin/) | Specifies the left margin of the paragraph. |
|[SetLeftMargin](./setleftmargin/) | Specifies the left margin of the paragraph. |
|[GetFirstLineIndent](./getfirstlineindent/) | Specifies the indent size that will be applied to the first line of text in the paragraph. |
|[SetFirstLineIndent](./setfirstlineindent/) | Specifies the indent size that will be applied to the first line of text in the paragraph. |
|[GetFontAlignType](./getfontaligntype/) | Determines where vertically on a line of text the actual words are positioned. This dealswith vertical placement of the characters with respect to the baselines. |
|[SetFontAlignType](./setfontaligntype/) | Determines where vertically on a line of text the actual words are positioned. This dealswith vertical placement of the characters with respect to the baselines. |
|[GetAlignmentType](./getalignmenttype/) | Gets and sets the text horizontal alignment type of the paragraph. |
|[SetAlignmentType](./setalignmenttype/) | Gets and sets the text horizontal alignment type of the paragraph. |
|[GetDefaultTabSize](./getdefaulttabsize/) | Gets and sets the default size for a tab character within this paragraph. |
|[SetDefaultTabSize](./setdefaulttabsize/) | Gets and sets the default size for a tab character within this paragraph. |
|[GetChildren](./getchildren/) | Gets all text runs in this paragraph.If this paragraph is empty, return paragraph itself. |
|[GetStartIndex](./getstartindex/) | Gets the start index of the characters. |
|[GetLength](./getlength/) | Gets the length of the characters. |
|[GetFont](./getfont/) | Returns the font of this object. |
|[SetWordArtStyle](./setwordartstyle/) | Sets the preset WordArt style. |
|[GetTextOptions](./gettextoptions/) | Returns the text options. |
