---
title: Aspose::Cells::Drawing::ShapeCollection::AddWordArt method
linktitle: AddWordArt
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::ShapeCollection::AddWordArt method. Adds preset WordArt since Excel 2007.s in C++.'
type: docs
weight: 2400
url: /cpp/aspose.cells.drawing/shapecollection/addwordart/
---
## ShapeCollection::AddWordArt(PresetWordArtStyle, const U16String\&, int32_t, int32_t, int32_t, int32_t, int32_t, int32_t) method


Adds preset WordArt since Excel 2007.s.

```cpp
Shape Aspose::Cells::Drawing::ShapeCollection::AddWordArt(PresetWordArtStyle style, const U16String &text, int32_t topRow, int32_t top, int32_t leftColumn, int32_t left, int32_t height, int32_t width)
```


| Parameter | Type | Description |
| --- | --- | --- |
| style | PresetWordArtStyle | The preset WordArt [Style](../../../aspose.cells/style/). |
| text | const U16String\& | The text. |
| topRow | int32_t | Upper left row index. |
| top | int32_t | Represents the vertical offset of shape from its left row, in unit of pixel. |
| leftColumn | int32_t | Upper left column index. |
| left | int32_t | Represents the horizontal offset of shape from its left column, in unit of pixel. |
| height | int32_t | Represents the height of shape, in unit of pixel. |
| width | int32_t | Represents the width of shape, in unit of pixel. |

## ReturnValue




## Examples


```cpp
//add a WordArt
U16String val = u"WordArt";
Shape wordArt2 = shapes.AddWordArt(PresetWordArtStyle::WordArtStyle1, val, 3, 0, 3, 0, 50, 200);
```

## See Also

* Class [Shape](../../shape/)
* Enum [PresetWordArtStyle](../../presetwordartstyle/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [ShapeCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
## ShapeCollection::AddWordArt(PresetWordArtStyle, const char16_t*, int32_t, int32_t, int32_t, int32_t, int32_t, int32_t) method


Adds preset WordArt since Excel 2007.s.

```cpp
Shape Aspose::Cells::Drawing::ShapeCollection::AddWordArt(PresetWordArtStyle style, const char16_t *text, int32_t topRow, int32_t top, int32_t leftColumn, int32_t left, int32_t height, int32_t width)
```


| Parameter | Type | Description |
| --- | --- | --- |
| style | PresetWordArtStyle | The preset WordArt [Style](../../../aspose.cells/style/). |
| text | const char16_t* | The text. |
| topRow | int32_t | Upper left row index. |
| top | int32_t | Represents the vertical offset of shape from its left row, in unit of pixel. |
| leftColumn | int32_t | Upper left column index. |
| left | int32_t | Represents the horizontal offset of shape from its left column, in unit of pixel. |
| height | int32_t | Represents the height of shape, in unit of pixel. |
| width | int32_t | Represents the width of shape, in unit of pixel. |

## ReturnValue




## Examples


```cpp
    //add a WordArt
Shape wordArt2 = shapes.AddWordArt(PresetWordArtStyle::WordArtStyle1, u"WordArt", 3, 0, 3, 0, 50, 200);
```

## See Also

* Class [Shape](../../shape/)
* Enum [PresetWordArtStyle](../../presetwordartstyle/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [ShapeCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
