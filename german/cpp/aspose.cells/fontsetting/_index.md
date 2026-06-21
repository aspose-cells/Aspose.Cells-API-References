---
title: Aspose::Cells::FontSetting class
linktitle: FontSetting
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::FontSetting class. Represents a range of characters within the cell text in C++.'
type: docs
weight: 7000
url: /de/cpp/aspose.cells/fontsetting/
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
//Instanziieren eines Workbook-Objekts
Workbook workbook;

//Hinzufügen eines neuen Arbeitsblatts zum Excel-Objekt
workbook.GetWorksheets().Add();

//Abrufen der Referenz des neu hinzugefügten Arbeitsblatts durch Übergeben seines Blattindexes
Worksheet worksheet = workbook.GetWorksheets().Get(0);

//Zugriff auf die Zelle "A1" im Arbeitsblatt
Cell cell = worksheet.GetCells().Get(u"A1");

//Hinzufügen eines Werts zur Zelle "A1"
cell.PutValue(u"Visit Aspose!");

//getting charactor
FontSetting charactor = cell.Characters(6, 7);

//Setting the font of selected characters to bold
charactor.GetFont().SetIsBold(true);

//Setting the font color of selected characters to blue
charactor.GetFont().SetColor(Color{ 0xff, 0, 0, 0xff });//Blue

//Speichern der Excel-Datei
workbook.Save(u"book1.xls");

Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
