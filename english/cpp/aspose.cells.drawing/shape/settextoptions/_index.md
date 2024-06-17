---
title: Aspose::Cells::Drawing::Shape::SetTextOptions method
linktitle: SetTextOptions
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Shape::SetTextOptions method. Represents the text options of the shape in C++.'
type: docs
weight: 15500
url: /cpp/aspose.cells.drawing/shape/settextoptions/
---
## Shape::SetTextOptions method


Represents the text options of the shape.

```cpp
void Aspose::Cells::Drawing::Shape::SetTextOptions(const TextOptions &value)
```


## Examples


```cpp
TextOptions opt = shape.GetTextOptions();
opt.SetColor(Color{ 0xff, 0, 0, 0xff });
opt.SetSize(8);
shape.SetTextOptions(opt);
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [TextOptions](../../../aspose.cells.drawing.texts/textoptions/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
