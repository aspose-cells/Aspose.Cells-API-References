##Aspose::Cells::Font class
'Aspose::Cells::Font class. Encapsulates the font object used in a spreadsheet in C++.'
## Font class
Encapsulates the font object used in a spreadsheet.
```cpp
class Font
```
## Methods
| Method | Description |
| --- | --- |
| [Equals(const Aspose::Cells::Font\& font)](./equals/) | Checks if two fonts are equals. |
| [Font(Font_Impl* impl)](./font/) | Constructs from an implementation object. |
| [Font(const Aspose::Cells::Font\& src)](./font/) | Copy constructor. |
| [GetArgbColor()](./getargbcolor/) | Gets and sets the color with a 32-bit ARGB value. |
| [GetCapsType()](./getcapstype/) | Gets and sets the text caps type. |
| [GetCharset()](./getcharset/) | Represent the character set. |
| [GetColor()](./getcolor/) | Gets or sets the [Color](../color/) of the font. |
| [GetDoubleSize()](./getdoublesize/) | Gets and sets the double size of the font. |
| [GetName()](./getname/) | Gets or sets the name of the [Font](./). |
| [GetSchemeType()](./getschemetype/) | Gets and sets the scheme type of the font. |
| [GetScriptOffset()](./getscriptoffset/) | Gets and sets the script offset,in unit of percentage. |
| [GetSize()](./getsize/) | Gets or sets the size of the font. |
| [GetStrikeType()](./getstriketype/) | Gets the strike type of the text. |
| [GetThemeColor()](./getthemecolor/) | Gets and sets the theme color. |
| [GetUnderline()](./getunderline/) | Gets or sets the font underline type. |
| [IsBold()](./isbold/) | Gets or sets a value indicating whether the font is bold. |
| [IsItalic()](./isitalic/) | Gets or sets a value indicating whether the font is italic. |
| [IsNormalizeHeights()](./isnormalizeheights/) | Indicates whether the normalization of height that is to be applied to the text run. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [IsStrikeout()](./isstrikeout/) | Gets or sets a value indicating whether the font is single strikeout. |
| [IsSubscript()](./issubscript/) | Gets or sets a value indicating whether the font is subscript. |
| [IsSuperscript()](./issuperscript/) | Gets or sets a value indicating whether the font is super script. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const Aspose::Cells::Font\& src)](./operator_asm/) | operator= |
| [SetArgbColor(int32_t value)](./setargbcolor/) | Gets and sets the color with a 32-bit ARGB value. |
| [SetCapsType(TextCapsType value)](./setcapstype/) | Gets and sets the text caps type. |
| [SetCharset(int32_t value)](./setcharset/) | Represent the character set. |
| [SetColor(const Aspose::Cells::Color\& value)](./setcolor/) | Gets or sets the [Color](../color/) of the font. |
| [SetDoubleSize(double value)](./setdoublesize/) | Gets and sets the double size of the font. |
| [SetIsBold(bool value)](./setisbold/) | Gets or sets a value indicating whether the font is bold. |
| [SetIsItalic(bool value)](./setisitalic/) | Gets or sets a value indicating whether the font is italic. |
| [SetIsNormalizeHeights(bool value)](./setisnormalizeheights/) | Indicates whether the normalization of height that is to be applied to the text run. |
| [SetIsStrikeout(bool value)](./setisstrikeout/) | Gets or sets a value indicating whether the font is single strikeout. |
| [SetIsSubscript(bool value)](./setissubscript/) | Gets or sets a value indicating whether the font is subscript. |
| [SetIsSuperscript(bool value)](./setissuperscript/) | Gets or sets a value indicating whether the font is super script. |
| [SetName(const U16String\& value)](./setname/) | Gets or sets the name of the [Font](./). |
| [SetName(const char16_t* value)](./setname/) | Gets or sets the name of the [Font](./). |
| [SetSchemeType(FontSchemeType value)](./setschemetype/) | Gets and sets the scheme type of the font. |
| [SetScriptOffset(double value)](./setscriptoffset/) | Gets and sets the script offset,in unit of percentage. |
| [SetSize(int32_t value)](./setsize/) | Gets or sets the size of the font. |
| [SetStrikeType(TextStrikeType value)](./setstriketype/) | Gets the strike type of the text. |
| [SetThemeColor(const ThemeColor\& value)](./setthemecolor/) | Gets and sets the theme color. |
| [SetUnderline(FontUnderlineType value)](./setunderline/) | Gets or sets the font underline type. |
| [ToString()](./tostring/) | Returns a string represents the current [Cell](../cell/) object. |
| [~Font()](./~font/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
Aspose::Cells::Startup();
//Instantiating a Workbook object
Workbook workbook;
//Obtaining the reference of the newly added worksheet by passing its sheet index
Worksheet worksheet = workbook.GetWorksheets().Get(0);
//Accessing the "A1" cell from the worksheet
Cell cell = worksheet.GetCells().Get(u"A1");
//Adding some value to the "A1" cell
cell.PutValue(u"Hello Aspose!");
Font font = cell.GetStyle().GetFont();
//Setting the font name to "Times New Roman"
font.SetName(u"Times New Roman");
//Setting font size to 14
font.SetSize(14);
//setting font color as Red
font.SetColor(Color{ 0xff, 0xff, 0, 0 });//Red
//Saving the Excel file
workbook.Save(u"dest.xls");
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
