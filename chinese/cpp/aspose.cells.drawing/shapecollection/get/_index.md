---
title: Aspose::Cells::Drawing::ShapeCollection::Get method
linktitle: Get
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::ShapeCollection::Get method. Gets the Shape object at the specific index in the list in C++.'
type: docs
weight: 600
url: /zh/cpp/aspose.cells.drawing/shapecollection/get/
---
## ShapeCollection::Get(int32_t) method


Gets the [Shape](../../shape/) object at the specific index in the list.

```cpp
Shape Aspose::Cells::Drawing::ShapeCollection::Get(int32_t index)
```


| Parameter | Type | Description |
| --- | --- | --- |
| index | int32_t | The index. |

## ReturnValue




## Examples


```cpp
//获取第一个形状
Shape shape = shapes.Get(0);
```

## See Also

* Class [Shape](../../shape/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [ShapeCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
## ShapeCollection::Get(const U16String\&) method


Gets the [Shape](../../shape/) object by the name of the shape.

```cpp
Shape Aspose::Cells::Drawing::ShapeCollection::Get(const U16String &name)
```


| Parameter | Type | Description |
| --- | --- | --- |
| name | const U16String\& | The name of the shape. |

## ReturnValue




## Examples


```cpp
    //添加形状
shapes.AddRectangle(2, 0, 2, 0, 130, 130);
//按名称获取形状。
U16String val = u"Rectangle 1";
Shape shape1 = shapes.Get(val);
if (!shape1.IsNull())
{
    //获取名为 'Rectangle 1' 的形状。
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


Gets the [Shape](../../shape/) object by the name of the shape.

```cpp
Shape Aspose::Cells::Drawing::ShapeCollection::Get(const char16_t *name)
```


| Parameter | Type | Description |
| --- | --- | --- |
| name | const char16_t* | The name of the shape. |

## ReturnValue




## Examples


```cpp
    //添加形状
shapes.AddRectangle(2, 0, 2, 0, 130, 130);
//获取形状
Shape shape1 = shapes.Get(u"Rectangle 1");
if (!shape1.IsNull())
{
    //获取名为 'Rectangle 1' 的形状。
}
```

## See Also

* Class [Shape](../../shape/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [ShapeCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
