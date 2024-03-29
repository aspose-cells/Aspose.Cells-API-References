---
title: Comment.ThreadedComments
second_title: Aspose.Cells for .NET API Reference
description: Comment property. Gets the list of threaded comments
type: docs
url: /net/aspose.cells/comment/threadedcomments/
---
## Comment.ThreadedComments property

Gets the list of threaded comments;

```csharp
public ThreadedCommentCollection ThreadedComments { get; }
```

### Examples

```csharp

[C#]
ThreadedCommentCollection threadedComments = comment1.ThreadedComments;
for (int i = 0; i < threadedComments.Count; ++i)
{
    ThreadedComment tc = threadedComments[i];
    string note = tc.Notes;
}
```

### See Also

* class [ThreadedCommentCollection](../../threadedcommentcollection/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


