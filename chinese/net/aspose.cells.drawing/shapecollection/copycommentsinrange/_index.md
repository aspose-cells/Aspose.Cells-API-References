---
title: CopyCommentsInRange
second_title: Aspose.Cells for .NET API 参考
description: 复制范围内的所有注释
type: docs
weight: 370
url: /zh/net/aspose.cells.drawing/shapecollection/copycommentsinrange/
---
## ShapeCollection.CopyCommentsInRange method

复制范围内的所有注释。

```csharp
public void CopyCommentsInRange(ShapeCollection shapes, CellArea ca, int destRow, int destColumn)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| shapes | ShapeCollection | 源形状。 |
| ca | CellArea | 源范围。 |
| destRow | Int32 | dest 范围起始行。 |
| destColumn | Int32 | dest 范围起始列。 |

### 例子

```csharp

[C#]
CommentCollection comments = workbook.Worksheets[0].Comments;

 //给单元格A1

int commentIndex = comments.Add(0, 0);
Comment comment = comments[commentIndex];
comment.Note = "First note.";
comment.Font.Name = "Times New Roman";

//向单元格B2

comments.Add("B2");
comment = comments["B2"];
comment.Note = "Second note.";

CellArea area1 = new CellArea();
area1.StartColumn = 1;
area1.StartRow = 1;
area1.EndColumn = 5;
area1.EndRow = 4;

 //copy
shapes.CopyCommentsInRange(shapes, area1, 5, 1);

```

### 也可以看看

* struct [CellArea](../../../aspose.cells/cellarea)
* class [ShapeCollection](../../shapecollection)
* 命名空间 [Aspose.Cells.Drawing](../../shapecollection)
* 部件 [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->