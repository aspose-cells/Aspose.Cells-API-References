---
title: Aspose::Cells::Drawing::Shape::GetTextBoxOptions method
linktitle: GetTextBoxOptions
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Shape::GetTextBoxOptions method. Gets the text information in the shape in C++.'
type: docs
weight: 18000
url: /cpp/aspose.cells.drawing/shape/gettextboxoptions/
---
## Shape::GetTextBoxOptions method


Gets the text information in the shape.

```cpp
TextBoxOptions Aspose::Cells::Drawing::Shape::GetTextBoxOptions()
```


## Examples


```cpp
TextBoxOptions textBoxOpt = shape.GetTextBoxOptions();
textBoxOpt.SetShapeTextVerticalAlignment(ShapeTextVerticalAlignmentType::Left);
textBoxOpt.SetTopMarginPt(0.2);
textBoxOpt.SetLeftMarginPt(0.2);
textBoxOpt.SetRightMarginPt(0.2);
textBoxOpt.SetBottomMarginPt(0.2);
```

## See Also

* Class [TextBoxOptions](../../../aspose.cells.drawing.texts/textboxoptions/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
