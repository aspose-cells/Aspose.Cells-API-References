---
title: Aspose::Cells::BorderCollection class
linktitle: BorderCollection
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::BorderCollection class. Encapsulates a collection of Border objects in C++.'
type: docs
weight: 1000
url: /fr/cpp/aspose.cells/bordercollection/
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
//Instanciation d'un objet Workbook
Workbook workbook;

//Ajout d'une nouvelle feuille de calcul à l'objet Excel
workbook.GetWorksheets().Add();

//Obtention de la référence de la feuille de calcul nouvellement ajoutée en passant son index de feuille
Worksheet worksheet = workbook.GetWorksheets().Get(0);

//Accès à la cellule "A1" de la feuille de calcul
Cell cell = worksheet.GetCells().Get(u"A1");

//Ajout d'une valeur à la cellule "A1"
cell.PutValue(u"Visit Aspose!");

Style style = cell.GetStyle();

//Définition du style de ligne de la bordure supérieure
style.GetBorders().Get(BorderType::TopBorder).SetLineStyle(CellBorderType::Thick);

//Définition de la couleur de la bordure supérieure
style.GetBorders().Get(BorderType::TopBorder).SetColor(Color{ 0xff, 0, 0, 0 });//Black

//Définition du style de ligne de la bordure inférieure
style.GetBorders().Get(BorderType::BottomBorder).SetLineStyle(CellBorderType::Thick);

//Définition de la couleur de la bordure inférieure
style.GetBorders().Get(BorderType::BottomBorder).SetColor(Color{ 0xff, 0, 0, 0 });//Black

//Définition du style de ligne de la bordure gauche
style.GetBorders().Get(BorderType::LeftBorder).SetLineStyle(CellBorderType::Thick);

//Définition de la couleur de la bordure gauche
style.GetBorders().Get(BorderType::LeftBorder).SetColor(Color{ 0xff, 0, 0, 0 });//Black

//Définition du style de ligne de la bordure droite
style.GetBorders().Get(BorderType::RightBorder).SetLineStyle(CellBorderType::Thick);

//Définir la couleur de la bordure droite
style.GetBorders().Get(BorderType::RightBorder).SetColor(Color{ 0xff, 0, 0, 0 });//Black

cell.SetStyle(style);

//Enregistrement du fichier Excel
workbook.Save(u"book1.xls");

Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
