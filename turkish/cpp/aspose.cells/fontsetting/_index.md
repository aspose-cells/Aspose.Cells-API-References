---
title: Aspose::Cells::FontSetting class
linktitle: FontSetting
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::FontSetting class. Represents a range of characters within the cell text in C++.'
type: docs
weight: 7000
url: /tr/cpp/aspose.cells/fontsetting/
---
## FontSetting class


Represents a range of characters within the cell text.

```cpp
class FontSetting
```

## Methods

| Method | Description |
| --- | --- |
| [FontSetting(int32_t startIndex, int32_t length, const WorksheetCollection\& sheets)](./fontsetting/) |  |
| [FontSetting(FontSetting_Impl* impl)](./fontsetting/) | Constructs from an implementation object. |
| [FontSetting(const FontSetting\& src)](./fontsetting/) | Copy constructor. |
| [GetFont()](./getfont/) | Returns the font of this object. |
| [GetLength()](./getlength/) | Gets the length of the characters. |
| [GetStartIndex()](./getstartindex/) | Gets the start index of the characters. |
| [GetTextOptions()](./gettextoptions/) | Returns the text options. |
| [GetType()](./gettype/) | Gets the type of text node. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const FontSetting\& src)](./operator_asm/) | operator= |
| [SetWordArtStyle(PresetWordArtStyle style)](./setwordartstyle/) | Sets the preset WordArt style. |
| [~FontSetting()](./~fontsetting/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |

## Examples


```cpp
Aspose::Cells::Startup();
//Bir Workbook nesnesi oluşturuluyor
Workbook workbook;

//Excel nesnesine yeni bir çalışma sayfası ekleniyor
workbook.GetWorksheets().Add();

//Yeni eklenen çalışma sayfasının referansını, sayfa indeksini geçirerek elde etme
Worksheet worksheet = workbook.GetWorksheets().Get(0);

//Çalışma sayfasından "A1" hücresine erişme
Cell cell = worksheet.GetCells().Get(u"A1");

//"A1" hücresine bir değer ekleme
cell.PutValue(u"Visit Aspose!");

//karakter al
FontSetting charactor = cell.Characters(6, 7);

//Seçili karakterlerin yazı tipini kalın olarak ayarla
charactor.GetFont().SetIsBold(true);

//Seçili karakterlerin yazı tipi rengini blue olarak ayarla
charactor.GetFont().SetColor(Color{ 0xff, 0, 0, 0xff });//Blue

//Excel dosyasını kaydetme
workbook.Save(u"book1.xls");

Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
