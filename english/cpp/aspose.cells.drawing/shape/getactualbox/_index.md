---
title: Aspose::Cells::Drawing::Shape::GetActualBox method
linktitle: GetActualBox
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Shape::GetActualBox method. Get the actual position and size of the shape (after applying rotation, flip, etc.) in C++.'
type: docs
weight: 19000
url: /cpp/aspose.cells.drawing/shape/getactualbox/
---
## Shape::GetActualBox method


Get the actual position and size of the shape (after applying rotation, flip, etc.)

```cpp
Vector<float> Aspose::Cells::Drawing::Shape::GetActualBox()
```


## ReturnValue

Return the position and size in the order of x, y, w, h
## Remarks



Note:The interface is not fully functional, especially the location information is not correct.It is recommended not to use this interface until the function is complete.

## Examples


```cpp
Vector<float> box = shape.GetActualBox();
std::cout << "x = " << box[0] << std::endl;
std::cout << "y = " << box[1] << std::endl;
std::cout << "w = " << box[2] << std::endl;
std::cout << "h = " << box[3] << std::endl;
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
