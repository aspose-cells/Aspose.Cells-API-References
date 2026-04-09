---
title: Aspose::Cells::Drawing::Shape::IsLocked method
linktitle: IsLocked
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Shape::IsLocked method. True means the object can not be modified when the sheet is protected. Note that this value is meaningful only if the worksheet or objects in the worksheet are protected in C++.'
type: docs
weight: 5100
url: /zh/cpp/aspose.cells.drawing/shape/islocked/
---
## Shape::IsLocked method


True means the object can not be modified when the sheet is protected. Note that this value is meaningful only if the worksheet or objects in the worksheet are protected.

```cpp
bool Aspose::Cells::Drawing::Shape::IsLocked()
```


## Examples


```cpp
//将指定的形状设置为未锁定状态
if (shape.GetWorksheet().IsProtected() && shape.IsLocked())
{
    shape.SetIsLocked(false);
}

//将指定的形状设置为锁定状态
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
