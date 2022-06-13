---
title: ThreadedComments
second_title: Aspose.Cells for .NET API 参考
description: 获取线程评论列表
type: docs
weight: 170
url: /zh/net/aspose.cells/comment/threadedcomments/
---
## Comment.ThreadedComments property

获取线程评论列表；

```csharp
public ThreadedCommentCollection ThreadedComments { get; }
```

### 例子

```csharp

[C#]
ThreadedCommentCollection threadedComments = comment1.ThreadedComments;
for (int i = 0; i < threadedComments.Count; ++i)
{
    ThreadedComment tc = threadedComments[i];
    string note = tc.Notes;
}
```

### 也可以看看

* class [ThreadedCommentCollection](../../threadedcommentcollection)
* class [Comment](../../comment)
* 命名空间 [Aspose.Cells](../../comment)
* 部件 [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->