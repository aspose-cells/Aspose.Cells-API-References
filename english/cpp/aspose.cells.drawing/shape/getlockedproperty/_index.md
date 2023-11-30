---
title: Aspose::Cells::Drawing::Shape::GetLockedProperty method
linktitle: GetLockedProperty
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Shape::GetLockedProperty method. Gets the value of locked property in C++.'
type: docs
weight: 3200
url: /cpp/aspose.cells.drawing/shape/getlockedproperty/
---
## Shape::GetLockedProperty method


Gets the value of locked property.

```cpp
bool Aspose::Cells::Drawing::Shape::GetLockedProperty(ShapeLockType type)
```


| Parameter | Type | Description |
| --- | --- | --- |
| type | ShapeLockType | The type of the shape locked property. |

## ReturnValue

Returns the value of locked property.


## Examples


```cpp
int noAdjustHandles = 0;
if (shape.GetLockedProperty(ShapeLockType::AdjustHandles))
    noAdjustHandles = 1;
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Enum [ShapeLockType](../../shapelocktype/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
