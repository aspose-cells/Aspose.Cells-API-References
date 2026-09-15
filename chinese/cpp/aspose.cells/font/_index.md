---
title: Aspose::Cells::Font class
linktitle: Font
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Font class. Encapsulates the font object used in a spreadsheet in C++.'
type: docs
weight: 6700
url: /zh/cpp/aspose.cells/font/
---
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
| [GetCapsType()](./getcapstype/) |  **(Deprecated)** Gets and sets the text caps type. |
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
| [IsNormalizeHeights()](./isnormalizeheights/) |  **(Deprecated)** Indicates whether the normalization of height that is to be applied to the text run. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [IsStrikeout()](./isstrikeout/) | Gets or sets a value indicating whether the font is single strikeout. |
| [IsSubscript()](./issubscript/) | Gets or sets a value indicating whether the font is subscript. |
| [IsSuperscript()](./issuperscript/) | Gets or sets a value indicating whether the font is super script. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const Aspose::Cells::Font\& src)](./operator_asm/) | operator= |
| [SetArgbColor(int32_t value)](./setargbcolor/) | Gets and sets the color with a 32-bit ARGB value. |
| [SetCapsType(TextCapsType value)](./setcapstype/) |  **(Deprecated)** Gets and sets the text caps type. |
| [SetCharset(int32_t value)](./setcharset/) | Represent the character set. |
| [SetColor(const Aspose::Cells::Color\& value)](./setcolor/) | Gets or sets the [Color](../color/) of the font. |
| [SetDoubleSize(double value)](./setdoublesize/) | Gets and sets the double size of the font. |
| [SetIsBold(bool value)](./setisbold/) | Gets or sets a value indicating whether the font is bold. |
| [SetIsItalic(bool value)](./setisitalic/) | Gets or sets a value indicating whether the font is italic. |
| [SetIsNormalizeHeights(bool value)](./setisnormalizeheights/) |  **(Deprecated)** Indicates whether the normalization of height that is to be applied to the text run. |
| [SetIsStrikeout(bool value)](./setisstrikeout/) | Gets or sets a value indicating whether the font is single strikeout. |
| [SetIsSubscript(bool value)](./setissubscript/) | Gets or sets a value indicating whether the font is subscript. |
| [SetIsSuperscript(bool value)](./setissuperscript/) | Gets or sets a value indicating whether the font is super script. |
| [SetName(const U16String\& name, FontSchemeType type)](./setname/) | Sets name and scheme of the font. |
| [SetName(const char16_t* name, FontSchemeType type)](./setname/) | Sets name and scheme of the font. |
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
//实例化 Workbook 对象
Workbook workbook;

//通过传递工作表索引获取新添加工作表的引用
Worksheet worksheet = workbook.GetWorksheets().Get(0);

//从工作表访问 "A1" 单元格
Cell cell = worksheet.GetCells().Get(u"A1");

//向 "A1" 单元格添加一些值
cell.PutValue(u"Hello Aspose!");

Font font = cell.GetStyle().GetFont();

//将字体名称设置为 "Times New Roman"
font.SetName(u"Times New Roman");

//将字体大小设置为 14
font.SetSize(14);

//将字体颜色设置为红色
font.SetColor(Color{ 0xff, 0xff, 0, 0 });//Red

//保存 Excel 文件
workbook.Save(u"dest.xls");

Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
