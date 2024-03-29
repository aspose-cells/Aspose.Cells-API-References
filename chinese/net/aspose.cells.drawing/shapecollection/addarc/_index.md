---
title: AddArc
second_title: Aspose.Cells for .NET API 参考
description: 将 ArcShape 添加到工作表
type: docs
weight: 30
url: /zh/net/aspose.cells.drawing/shapecollection/addarc/
---
## ShapeCollection.AddArc method

将 ArcShape 添加到工作表。

```csharp
public ArcShape AddArc(int upperLeftRow, int top, int upperLeftColumn, int left, int height, 
    int width)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| upperLeftRow | Int32 | 左上行索引。 |
| top | Int32 | 表示 ArcShape 与其左行的垂直偏移量，以像素为单位。 |
| upperLeftColumn | Int32 | 左上列索引。 |
| left | Int32 | 表示 ArcShape 与其左列的水平偏移量，以像素为单位。 |
| height | Int32 | 表示 ArcShape 的高度，以像素为单位。 |
| width | Int32 | 表示 ArcShape 的宽度，以像素为单位。 |

### 返回值

一个 ArcShape 对象。

### 例子

```csharp

[C#]
//添加一个弧
ArcShape arcShape = shapes.AddArc(1, 0, 1, 0, 100, 50);
```

### 也可以看看

* class [ArcShape](../../arcshape)
* class [ShapeCollection](../../shapecollection)
* 命名空间 [Aspose.Cells.Drawing](../../shapecollection)
* 部件 [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
