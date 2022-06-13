---
title: AddOval
second_title: Aspose.Cells for .NET API 参考
description: 向工作表添加椭圆
type: docs
weight: 200
url: /zh/net/aspose.cells.drawing/shapecollection/addoval/
---
## ShapeCollection.AddOval method

向工作表添加椭圆。

```csharp
public Oval AddOval(int upperLeftRow, int top, int upperLeftColumn, int left, int height, int width)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| upperLeftRow | Int32 | 左上行索引。 |
| top | Int32 | 表示 Oval 与其左行的垂直偏移量，以像素为单位。 |
| upperLeftColumn | Int32 | 左上列索引。 |
| left | Int32 | 表示 Oval 与其左列的水平偏移量，以像素为单位。 |
| height | Int32 | 表示椭圆的高度，以像素为单位。 |
| width | Int32 | 表示椭圆的宽度，以像素为单位。 |

### 返回值

椭圆形对象。

### 例子

```csharp

[C#]
 //添加一个椭圆形
Oval oval = shapes.AddOval(1, 0, 1, 0, 50, 50);
```

### 也可以看看

* class [Oval](../../oval)
* class [ShapeCollection](../../shapecollection)
* 命名空间 [Aspose.Cells.Drawing](../../shapecollection)
* 部件 [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->