---
title: "Comment.ThreadedComments"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Comment-Eigenschaft. Gibt die Liste der ThreadedComments zurück"
type: docs
url: /de/net/aspose.cells/comment/threadedcomments/
---
## Comment.ThreadedComments property

Liest die Liste der Threaded Comments;

```csharp
public ThreadedCommentCollection ThreadedComments { get; }
```

### Beispiele

```csharp

[C#]
ThreadedCommentCollection threadedComments = comment1.ThreadedComments;
for (int i = 0; i < threadedComments.Count; ++i)
{
    ThreadedComment tc = threadedComments[i];
    string note = tc.Notes;
}
```

### Siehe auch

* class [ThreadedCommentCollection](../../threadedcommentcollection/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


