---
title: Aspose::Cells::Drawing::ShapeCollection::AddTextEffect method
linktitle: AddTextEffect
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::ShapeCollection::AddTextEffect method. Inserts a WordArt object in C++.'
type: docs
weight: 2300
url: /cpp/aspose.cells.drawing/shapecollection/addtexteffect/
---
## ShapeCollection::AddTextEffect(MsoPresetTextEffect, const U16String\&, const U16String\&, int32_t, bool, bool, int32_t, int32_t, int32_t, int32_t, int32_t, int32_t) method


Inserts a WordArt object.

```cpp
Shape Aspose::Cells::Drawing::ShapeCollection::AddTextEffect(MsoPresetTextEffect effect, const U16String &text, const U16String &fontName, int32_t size, bool fontBold, bool fontItalic, int32_t topRow, int32_t top, int32_t leftColumn, int32_t left, int32_t height, int32_t width)
```


| Parameter | Type | Description |
| --- | --- | --- |
| effect | MsoPresetTextEffect | The mso preset text effect type. |
| text | const U16String\& | The WordArt text. |
| fontName | const U16String\& | The font name. |
| size | int32_t | The font size |
| fontBold | bool | Indicates whether font is bold. |
| fontItalic | bool | Indicates whether font is italic. |
| topRow | int32_t | Upper left row index. |
| top | int32_t | Represents the vertical offset of shape from its left row, in unit of pixel. |
| leftColumn | int32_t | Upper left column index. |
| left | int32_t | Represents the horizontal offset of shape from its left column, in unit of pixel. |
| height | int32_t | Represents the height of shape, in unit of pixel. |
| width | int32_t | Represents the width of shape, in unit of pixel. |

## ReturnValue

Returns a [Shape](../../shape/) object that represents the new WordArt object.


## Examples


```cpp
//add a WordArt
U16String txt = u"WordArt";
U16String fName = u"arial";
Shape wordArt1 = shapes.AddTextEffect(MsoPresetTextEffect::TextEffect10, txt, fName, 18, false, false, 3, 0, 3, 0, 200, 50);
```

## See Also

* Class [Shape](../../shape/)
* Enum [MsoPresetTextEffect](../../msopresettexteffect/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [ShapeCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
## ShapeCollection::AddTextEffect(MsoPresetTextEffect, const char16_t*, const char16_t*, int32_t, bool, bool, int32_t, int32_t, int32_t, int32_t, int32_t, int32_t) method


Inserts a WordArt object.

```cpp
Shape Aspose::Cells::Drawing::ShapeCollection::AddTextEffect(MsoPresetTextEffect effect, const char16_t *text, const char16_t *fontName, int32_t size, bool fontBold, bool fontItalic, int32_t topRow, int32_t top, int32_t leftColumn, int32_t left, int32_t height, int32_t width)
```


| Parameter | Type | Description |
| --- | --- | --- |
| effect | MsoPresetTextEffect | The mso preset text effect type. |
| text | const char16_t* | The WordArt text. |
| fontName | const char16_t* | The font name. |
| size | int32_t | The font size |
| fontBold | bool | Indicates whether font is bold. |
| fontItalic | bool | Indicates whether font is italic. |
| topRow | int32_t | Upper left row index. |
| top | int32_t | Represents the vertical offset of shape from its left row, in unit of pixel. |
| leftColumn | int32_t | Upper left column index. |
| left | int32_t | Represents the horizontal offset of shape from its left column, in unit of pixel. |
| height | int32_t | Represents the height of shape, in unit of pixel. |
| width | int32_t | Represents the width of shape, in unit of pixel. |

## ReturnValue

Returns a [Shape](../../shape/) object that represents the new WordArt object.


## Examples


```cpp
    //add a WordArt
Shape wordArt1 = shapes.AddTextEffect(MsoPresetTextEffect::TextEffect10, u"WordArt", u"arial", 18, false, false, 3, 0, 3, 0, 200, 50);
```

## See Also

* Class [Shape](../../shape/)
* Enum [MsoPresetTextEffect](../../msopresettexteffect/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [ShapeCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
