---
title: Aspose::Cells::Drawing::Texts::ShapeTextAlignment::GetTextShapeType method
linktitle: GetTextShapeType
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Texts::ShapeTextAlignment::GetTextShapeType method. Gets and set the transform type of text in C++.'
type: docs
weight: 2200
url: /es/cpp/aspose.cells.drawing.texts/shapetextalignment/gettextshapetype/
---
## ShapeTextAlignment::GetTextShapeType method


Gets and set the transform type of text.

```cpp
AutoShapeType Aspose::Cells::Drawing::Texts::ShapeTextAlignment::GetTextShapeType()
```


## Examples


```cpp
//Normalmente no modifique este valor a menos que sepa exactamente cuál será el resultado de la modificación
if (shapeTextAlignment.GetTextShapeType() == AutoShapeType::TextBox)
{
    shapeTextAlignment.SetTextShapeType(AutoShapeType::TextBox);
}
```

## See Also

* Enum [AutoShapeType](../../../aspose.cells.drawing/autoshapetype/)
* Class [ShapeTextAlignment](../)
* Namespace [Aspose::Cells::Drawing::Texts](../../)
* Library [Aspose.Cells for C++](../../../)
