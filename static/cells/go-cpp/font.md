##Font Class
'Font class. Encapsulates the object that represents font in Go.'
## Font class
Encapsulates the font object used in a spreadsheet.
```go
type Font struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetCharset](./getcharset/) | Represent the character set. |
|[SetCharset](./setcharset/) | Represent the character set. |
|[IsItalic](./isitalic/) | Gets or sets a value indicating whether the font is italic. |
|[SetIsItalic](./setisitalic/) | Gets or sets a value indicating whether the font is italic. |
|[IsBold](./isbold/) | Gets or sets a value indicating whether the font is bold. |
|[SetIsBold](./setisbold/) | Gets or sets a value indicating whether the font is bold. |
|[GetCapsType](./getcapstype/) | Gets and sets the text caps type. |
|[SetCapsType](./setcapstype/) | Gets and sets the text caps type. |
|[GetStrikeType](./getstriketype/) | Gets the strike type of the text. |
|[SetStrikeType](./setstriketype/) | Gets the strike type of the text. |
|[IsStrikeout](./isstrikeout/) | Gets or sets a value indicating whether the font is single strikeout. |
|[SetIsStrikeout](./setisstrikeout/) | Gets or sets a value indicating whether the font is single strikeout. |
|[GetScriptOffset](./getscriptoffset/) | Gets and sets the script offset,in unit of percentage |
|[SetScriptOffset](./setscriptoffset/) | Gets and sets the script offset,in unit of percentage |
|[IsSuperscript](./issuperscript/) | Gets or sets a value indicating whether the font is super script. |
|[SetIsSuperscript](./setissuperscript/) | Gets or sets a value indicating whether the font is super script. |
|[IsSubscript](./issubscript/) | Gets or sets a value indicating whether the font is subscript. |
|[SetIsSubscript](./setissubscript/) | Gets or sets a value indicating whether the font is subscript. |
|[GetUnderline](./getunderline/) | Gets or sets the font underline type. |
|[SetUnderline](./setunderline/) | Gets or sets the font underline type. |
|[GetDoubleSize](./getdoublesize/) | Gets and sets the double size of the font. |
|[SetDoubleSize](./setdoublesize/) | Gets and sets the double size of the font. |
|[GetSize](./getsize/) | Gets or sets the size of the font. |
|[SetSize](./setsize/) | Gets or sets the size of the font. |
|[GetThemeColor](./getthemecolor/) | Gets and sets the theme color. |
|[SetThemeColor](./setthemecolor/) | Gets and sets the theme color. |
|[GetColor](./getcolor/) | Gets or sets the Color of the font. |
|[SetColor](./setcolor/) | Gets or sets the Color of the font. |
|[GetArgbColor](./getargbcolor/) | Gets and sets the color with a 32-bit ARGB value. |
|[SetArgbColor](./setargbcolor/) | Gets and sets the color with a 32-bit ARGB value. |
|[Equals](./equals/) | Checks if two fonts are equals. |
|[IsNormalizeHeights](./isnormalizeheights/) | Indicates whether the normalization of height that is to be applied to the text run. |
|[SetIsNormalizeHeights](./setisnormalizeheights/) | Indicates whether the normalization of height that is to be applied to the text run. |
|[GetSchemeType](./getschemetype/) | Gets and sets the scheme type of the font. |
|[SetSchemeType](./setschemetype/) | Gets and sets the scheme type of the font. |
|[ToString](./tostring/) | Returns a string represents the current Cell object. |
|[GetName](./getname/) | Gets  or sets the name of the Font. |
|[SetName](./setname/) | Gets  or sets the name of the Font. |
