---
title: CopyInRange
second_title: Aspose.Cells for .NET API 参考
description: 将范围内的形状复制到目标范围
type: docs
weight: 380
url: /zh/net/aspose.cells.drawing/shapecollection/copyinrange/
---
## ShapeCollection.CopyInRange method

将范围内的形状复制到目标范围。

```csharp
public void CopyInRange(ShapeCollection sourceShapes, CellArea ca, int destRow, int destColumn, 
    bool isContained)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| sourceShapes | ShapeCollection | 源形状。 |
| ca | CellArea | 源范围。 |
| destRow | Int32 | dest 范围的 dest 行索引。 |
| destColumn | Int32 | dest 范围的 dest 列。 |
| isContained | Boolean | 是否只复制范围内包含的形状。 如果为真，则仅复制范围内的形状。 否则，它作为 MS Office 工作。 |

### 例子

```csharp

[C#]
 //添加一个shape
shapes.AddRectangle(2, 0, 2, 0, 130, 130);
CellArea area2 = new CellArea();
area2.StartColumn = 1;
area2.StartRow = 1;
area2.EndColumn = 5;
area2.EndRow = 11;

 //copy
shapes.CopyInRange(shapes, area2, 12, 1, false);

```

### 也可以看看

* struct [CellArea](../../../aspose.cells/cellarea)
* class [ShapeCollection](../../shapecollection)
* 命名空间 [Aspose.Cells.Drawing](../../shapecollection)
* 部件 [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->