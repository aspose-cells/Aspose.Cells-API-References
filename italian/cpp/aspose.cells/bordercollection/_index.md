---
title: Aspose::Cells::BorderCollection class
linktitle: BorderCollection
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::BorderCollection class. Encapsulates a collection of Border objects in C++.'
type: docs
weight: 1000
url: /it/cpp/aspose.cells/bordercollection/
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
//Istanziare un oggetto Workbook
Workbook workbook;

//Aggiungere un nuovo foglio di lavoro all'oggetto Excel
workbook.GetWorksheets().Add();

//Ottenere il riferimento del foglio di lavoro appena aggiunto passando il suo indice di foglio
Worksheet worksheet = workbook.GetWorksheets().Get(0);

//Accedere alla cella "A1" dal foglio di lavoro
Cell cell = worksheet.GetCells().Get(u"A1");

//Aggiungere un valore alla cella "A1"
cell.PutValue(u"Visit Aspose!");

Style style = cell.GetStyle();

//Impostare lo stile della linea del bordo superiore
style.GetBorders().Get(BorderType::TopBorder).SetLineStyle(CellBorderType::Thick);

//Impostare il colore del bordo superiore
style.GetBorders().Get(BorderType::TopBorder).SetColor(Color{ 0xff, 0, 0, 0 });//Black

//Impostare lo stile della linea del bordo inferiore
style.GetBorders().Get(BorderType::BottomBorder).SetLineStyle(CellBorderType::Thick);

//Impostare il colore del bordo inferiore
style.GetBorders().Get(BorderType::BottomBorder).SetColor(Color{ 0xff, 0, 0, 0 });//Black

//Impostare lo stile della linea del bordo sinistro
style.GetBorders().Get(BorderType::LeftBorder).SetLineStyle(CellBorderType::Thick);

//Impostare il colore del bordo sinistro
style.GetBorders().Get(BorderType::LeftBorder).SetColor(Color{ 0xff, 0, 0, 0 });//Black

//Impostare lo stile della linea del bordo destro
style.GetBorders().Get(BorderType::RightBorder).SetLineStyle(CellBorderType::Thick);

//Setting the color of the right border
style.GetBorders().Get(BorderType::RightBorder).SetColor(Color{ 0xff, 0, 0, 0 });//Black

cell.SetStyle(style);

//Saving the Excel file
workbook.Save(u"book1.xls");

Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
