---
title: Remove
second_title: Aspose.Cells for .NET API 参考
description: 移除形状
type: docs
weight: 420
url: /zh/net/aspose.cells.drawing/shapecollection/remove/
---
## ShapeCollection.Remove method

移除形状。

```csharp
public void Remove(Shape shape)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| shape | Shape |  |

### 例子

```csharp

[C#]
//添加第一个形状
shapes.AddRectangle(2, 0, 2, 0, 50, 50);
//添加第二个形状
shapes.AddRectangle(6, 0, 2, 0, 30, 30);

//获取形状
Shape s = shapes["Rectangle 1"];// 或形状[0];
if (s != null)
{
    //消除 
    shapes.Remove(s);
}
```

### 也可以看看

* class [Shape](../../shape)
* class [ShapeCollection](../../shapecollection)
* 命名空间 [Aspose.Cells.Drawing](../../shapecollection)
* 部件 [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
