---
title: Aspose::Cells::Drawing::ShapeCollection::Get method
linktitle: Get
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::ShapeCollection::Get method. Gets the shape object at the specific index in C++.'
type: docs
weight: 600
url: /cpp/aspose.cells.drawing/shapecollection/get/
---
## ShapeCollection::Get(int32_t) method


Gets the shape object at the specific index.

```cpp
Shape Aspose::Cells::Drawing::ShapeCollection::Get(int32_t index)
```


| Parameter | Type | Description |
| --- | --- | --- |
| index | int32_t |  |

## ReturnValue




## Examples


```cpp
    //get the shape
Shape shape = shapes.Get(shapes.GetCount() - 1);
```

## See Also

* Class [Shape](../../shape/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [ShapeCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
## ShapeCollection::Get(const U16String\&) method


Gets the shape object by the shape image.

```cpp
Shape Aspose::Cells::Drawing::ShapeCollection::Get(const U16String &name)
```


| Parameter | Type | Description |
| --- | --- | --- |
| name | const U16String\& |  |

## ReturnValue




## Examples


```cpp
    //add a shape
shapes.AddRectangle(2, 0, 2, 0, 130, 130);
//get the shape
U16String val = u"Rectangle 1";
Shape shape1 = shapes.Get(val);
if (!shape1.IsNull())
{
    //Got the shape named 'Rectangle 1'.
}
```

## See Also

* Class [Shape](../../shape/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [ShapeCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
## ShapeCollection::Get(const char16_t*) method


Gets the shape object by the shape image.

```cpp
Shape Aspose::Cells::Drawing::ShapeCollection::Get(const char16_t *name)
```


| Parameter | Type | Description |
| --- | --- | --- |
| name | const char16_t* |  |

## ReturnValue




## Examples


```cpp
    //add a shape
shapes.AddRectangle(2, 0, 2, 0, 130, 130);
//get the shape
Shape shape1 = shapes.Get(u"Rectangle 1");
if (!shape1.IsNull())
{
    //Got the shape named 'Rectangle 1'.
}
```

## See Also

* Class [Shape](../../shape/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [ShapeCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
