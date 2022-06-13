---
title: AddLabel
second_title: Aspose.Cells for .NET API 参考
description: 向工作表添加标签
type: docs
weight: 130
url: /zh/net/aspose.cells.drawing/shapecollection/addlabel/
---
## ShapeCollection.AddLabel method

向工作表添加标签。

```csharp
public Label AddLabel(int upperLeftRow, int top, int upperLeftColumn, int left, int height, 
    int width)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| upperLeftRow | Int32 | 左上行索引。 |
| top | Int32 | 表示Label相对左行的垂直偏移量，以像素为单位。 |
| upperLeftColumn | Int32 | 左上列索引。 |
| left | Int32 | 表示Label从其左列的水平偏移量，以像素为单位。 |
| height | Int32 | 表示Label的高度，以像素为单位。 |
| width | Int32 | 表示Label的宽度，以像素为单位。 |

### 返回值

标签对象。

### 例子

```csharp

[C#]
 //添加一个标签
Label label = shapes.AddLabel(1, 0, 1, 0, 100, 50);
```

### 也可以看看

* class [Label](../../label)
* class [ShapeCollection](../../shapecollection)
* 命名空间 [Aspose.Cells.Drawing](../../shapecollection)
* 部件 [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->