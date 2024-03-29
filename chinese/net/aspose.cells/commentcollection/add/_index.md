---
title: Add
second_title: Aspose.Cells for .NET API 参考
description: 向集合添加评论
type: docs
weight: 20
url: /zh/net/aspose.cells/commentcollection/add/
---
## Add(int, int) {#add}

向集合添加评论。

```csharp
public int Add(int row, int column)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| row | Int32 | 单元格行索引。 |
| column | Int32 | 单元格列索引。 |

### 返回值

[`Comment`](../../comment)对象索引。

### 例子

```csharp

[C#]
int commentIndex1 = comments.Add(0, 0);
Comment comment1 = comments[commentIndex1];
comment1.Note = "First note.";
comment1.Font.Name = "Times New Roman";
```

### 也可以看看

* class [CommentCollection](../../commentcollection)
* 命名空间 [Aspose.Cells](../../commentcollection)
* 部件 [Aspose.Cells](../../../)

---

## Add(string) {#add_1}

向集合添加评论。

```csharp
public int Add(string cellName)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| cellName | String | 单元格名称。 |

### 返回值

[`Comment`](../../comment)对象索引。

### 例子

```csharp

[C#]
int commentIndex2 = comments.Add("B2");
Comment comment2 = comments[commentIndex2];
comment2.Note = "Second note.";
comment2.Font.Name = "Times New Roman";
```

### 也可以看看

* class [CommentCollection](../../commentcollection)
* 命名空间 [Aspose.Cells](../../commentcollection)
* 部件 [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
