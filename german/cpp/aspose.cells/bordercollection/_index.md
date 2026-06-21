---
title: Aspose::Cells::BorderCollection class
linktitle: BorderCollection
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::BorderCollection class. Encapsulates a collection of Border objects in C++.'
type: docs
weight: 1000
url: /de/cpp/aspose.cells/bordercollection/
---
## BorderCollection class


Encapsulates a collection of [Border](../border/) objects.

```cpp
class BorderCollection
```

## Methods

| Method | Description |
| --- | --- |
| [BorderCollection(BorderCollection_Impl* impl)](./bordercollection/) | Constructs from an implementation object. |
| [BorderCollection(const BorderCollection\& src)](./bordercollection/) | Copy constructor. |
| [Get(BorderType borderType)](./get/) | Gets the [Border](../border/) element at the specified index. |
| [GetDiagonalColor()](./getdiagonalcolor/) | Gets or sets the [Color](../color/) of Diagonal lines. |
| [GetDiagonalStyle()](./getdiagonalstyle/) | Gets or sets the style of Diagonal lines. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const BorderCollection\& src)](./operator_asm/) | operator= |
| [SetColor(const Aspose::Cells::Color\& color)](./setcolor/) | Sets the [Color](../color/) of all borders in the collection. |
| [SetDiagonalColor(const Aspose::Cells::Color\& value)](./setdiagonalcolor/) | Gets or sets the [Color](../color/) of Diagonal lines. |
| [SetDiagonalStyle(CellBorderType value)](./setdiagonalstyle/) | Gets or sets the style of Diagonal lines. |
| [SetStyle(CellBorderType style)](./setstyle/) | Sets the style of all borders of the collection. |
| [~BorderCollection()](./~bordercollection/) | Destructor. |
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

Style style = cell.GetStyle();

//Festlegen des Linienstils des oberen Rahmens
style.GetBorders().Get(BorderType::TopBorder).SetLineStyle(CellBorderType::Thick);

//Festlegen der Farbe des oberen Rahmens
style.GetBorders().Get(BorderType::TopBorder).SetColor(Color{ 0xff, 0, 0, 0 });//Black

//Festlegen des Linienstils des unteren Rahmens
style.GetBorders().Get(BorderType::BottomBorder).SetLineStyle(CellBorderType::Thick);

//Festlegen der Farbe des unteren Rahmens
style.GetBorders().Get(BorderType::BottomBorder).SetColor(Color{ 0xff, 0, 0, 0 });//Black

//Festlegen des Linienstils des linken Rahmens
style.GetBorders().Get(BorderType::LeftBorder).SetLineStyle(CellBorderType::Thick);

//Festlegen der Farbe des linken Rahmens
style.GetBorders().Get(BorderType::LeftBorder).SetColor(Color{ 0xff, 0, 0, 0 });//Black

//Festlegen des Linienstils des rechten Rahmens
style.GetBorders().Get(BorderType::RightBorder).SetLineStyle(CellBorderType::Thick);

//Festlegen der Farbe des rechten Randes
style.GetBorders().Get(BorderType::RightBorder).SetColor(Color{ 0xff, 0, 0, 0 });//Black

cell.SetStyle(style);

//Speichern der Excel-Datei
workbook.Save(u"book1.xls");

Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
