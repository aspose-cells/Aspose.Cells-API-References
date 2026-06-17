---
title: Aspose::Cells::BorderCollection class
linktitle: BorderCollection
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::BorderCollection class. Encapsulates a collection of Border objects in C++.'
type: docs
weight: 1000
url: /ru/cpp/aspose.cells/bordercollection/
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
//Создание экземпляра объекта Workbook
Workbook workbook;

//Добавление нового листа в объект Excel
workbook.GetWorksheets().Add();

//Получение ссылки на только что добавленный лист путем передачи его индекса листа
Worksheet worksheet = workbook.GetWorksheets().Get(0);

//Доступ к ячейке "A1" листа
Cell cell = worksheet.GetCells().Get(u"A1");

//Добавление некоторого значения в ячейку "A1"
cell.PutValue(u"Visit Aspose!");

Style style = cell.GetStyle();

//Установка стиля линии верхней границы
style.GetBorders().Get(BorderType::TopBorder).SetLineStyle(CellBorderType::Thick);

//Установка цвета верхней границы
style.GetBorders().Get(BorderType::TopBorder).SetColor(Color{ 0xff, 0, 0, 0 });//Black

//Установка стиля линии нижней границы
style.GetBorders().Get(BorderType::BottomBorder).SetLineStyle(CellBorderType::Thick);

//Установка цвета нижней границы
style.GetBorders().Get(BorderType::BottomBorder).SetColor(Color{ 0xff, 0, 0, 0 });//Black

//Установка стиля линии левой границы
style.GetBorders().Get(BorderType::LeftBorder).SetLineStyle(CellBorderType::Thick);

//Установка цвета левой границы
style.GetBorders().Get(BorderType::LeftBorder).SetColor(Color{ 0xff, 0, 0, 0 });//Black

//Установка стиля линии правой границы
style.GetBorders().Get(BorderType::RightBorder).SetLineStyle(CellBorderType::Thick);

//Установка цвета правой границы
style.GetBorders().Get(BorderType::RightBorder).SetColor(Color{ 0xff, 0, 0, 0 });//Black

cell.SetStyle(style);

//Сохранение файла Excel
workbook.Save(u"book1.xls");

Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
