---
title: CommentCollection.GetThreadedComments
second_title: Aspose.Cells for .NET API Reference
description: CommentCollection method. Gets the threaded comments by row and column index
type: docs
url: /net/aspose.cells/commentcollection/getthreadedcomments/
---
## GetThreadedComments(int, int) {#getthreadedcomments}

Gets the threaded comments by row and column index.

```csharp
public ThreadedCommentCollection GetThreadedComments(int row, int column)
```

| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | The row index. |
| column | Int32 | The column index. |

### Examples

```csharp

[C#]
ThreadedCommentCollection threadedComments1 = comments.GetThreadedComments(1, 1);
for (int i = 0; i < threadedComments1.Count; ++i)
{
    ThreadedComment tc = threadedComments1[i];
    string note = tc.Notes;
}
```

### See Also

* class [ThreadedCommentCollection](../../threadedcommentcollection/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetThreadedComments(string) {#getthreadedcomments_1}

Gets the threaded comments by cell name.

```csharp
public ThreadedCommentCollection GetThreadedComments(string cellName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| cellName | String | The name of the cell. |

### Examples

```csharp

[C#]
ThreadedCommentCollection threadedComments2 = comments.GetThreadedComments("B2");
for (int i = 0; i < threadedComments2.Count; ++i)
{
    ThreadedComment tc = threadedComments2[i];
    string note = tc.Notes;
}
```

### See Also

* class [ThreadedCommentCollection](../../threadedcommentcollection/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


