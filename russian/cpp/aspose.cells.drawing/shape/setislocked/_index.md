---
title: Aspose::Cells::Drawing::Shape::SetIsLocked method
linktitle: SetIsLocked
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Shape::SetIsLocked method. True means the object can not be modified when the sheet is protected. Note that this value is meaningful only if the worksheet or objects in the worksheet are protected in C++.'
type: docs
weight: 5200
url: /ru/cpp/aspose.cells.drawing/shape/setislocked/
---
## Shape::SetIsLocked method


True means the object can not be modified when the sheet is protected. Note that this value is meaningful only if the worksheet or objects in the worksheet are protected.

```cpp
void Aspose::Cells::Drawing::Shape::SetIsLocked(bool value)
```


## Examples


```cpp
//Устанавливает указанную фигуру в разблокированное состояние
if (shape.GetWorksheet().IsProtected() && shape.IsLocked())
{
    shape.SetIsLocked(false);
}

//Устанавливает указанную фигуру в заблокированное состояние
if (shape.GetWorksheet().IsProtected() && !shape.IsLocked())
{
    shape.SetIsLocked(true);
}
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
