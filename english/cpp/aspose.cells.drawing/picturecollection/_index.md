---
title: Aspose::Cells::Drawing::PictureCollection class
linktitle: PictureCollection
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::PictureCollection class. Encapsulates a collection of Picture objects in C++.'
type: docs
weight: 4500
url: /cpp/aspose.cells.drawing/picturecollection/
---
## PictureCollection class


Encapsulates a collection of [Picture](../picture/) objects.

```cpp
class PictureCollection
```

## Methods

| Method | Description |
| --- | --- |
| [Add(int32_t topRow, int32_t leftColumn, int32_t bottomRow, int32_t rightColumn, const Vector \<uint8_t\>\& stream)](./add/) | Adds a picture to the collection. |
| [Add(int32_t topRow, int32_t leftColumn, int32_t bottomRow, int32_t rightColumn, const U16String\& fileName)](./add/) | Adds a picture to the collection. |
| [Add(int32_t topRow, int32_t leftColumn, int32_t bottomRow, int32_t rightColumn, const char16_t* fileName)](./add/) | Adds a picture to the collection. |
| [Add(int32_t topRow, int32_t leftColumn, const Vector \<uint8_t\>\& stream)](./add/) | Adds a picture to the collection. |
| [Add(int32_t topRow, int32_t leftColumn, const U16String\& fileName)](./add/) | Adds a picture to the collection. |
| [Add(int32_t topRow, int32_t leftColumn, const char16_t* fileName)](./add/) | Adds a picture to the collection. |
| [Add(int32_t topRow, int32_t leftColumn, const Vector \<uint8_t\>\& stream, int32_t widthScale, int32_t heightScale)](./add/) | Adds a picture to the collection. |
| [Add(int32_t topRow, int32_t leftColumn, const U16String\& fileName, int32_t widthScale, int32_t heightScale)](./add/) | Adds a picture to the collection. |
| [Add(int32_t topRow, int32_t leftColumn, const char16_t* fileName, int32_t widthScale, int32_t heightScale)](./add/) | Adds a picture to the collection. |
| [Camera(int32_t row, int32_t column, const U16String\& range)](./camera/) | Takes a photo of the range. |
| [Camera(int32_t row, int32_t column, const char16_t* range)](./camera/) | Takes a photo of the range. |
| [Clear()](./clear/) | Clear all pictures. |
| [Get(int32_t index)](./get/) | Gets the [Picture](../picture/) element at the specified index. |
| [GetCount()](./getcount/) |  |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const PictureCollection\& src)](./operator_asm/) | operator= |
| [PictureCollection(PictureCollection_Impl* impl)](./picturecollection/) | Constructs from an implementation object. |
| [PictureCollection(const PictureCollection\& src)](./picturecollection/) | Copy constructor. |
| [RemoveAt(int32_t index)](./removeat/) | Remove shapes at the specific index. |
| [~PictureCollection()](./~picturecollection/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |

## Examples


```cpp
Aspose::Cells::Startup();
//Instantiating a Workbook object
Workbook workbook;

//get PictureCollection
PictureCollection pictures = workbook.GetWorksheets().Get(0).GetPictures();


//Save the excel file.
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells::Drawing](../)
* Library [Aspose.Cells for C++](../../)
