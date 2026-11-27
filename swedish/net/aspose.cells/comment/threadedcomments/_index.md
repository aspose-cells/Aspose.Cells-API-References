---
title: "Comment.ThreadedComments"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Comment property. Hämtar listan med trådade kommentarer"
type: docs
url: /sv/net/aspose.cells/comment/threadedcomments/
---
## Comment.ThreadedComments property

Hämtar listan över trådade kommentarer;

```csharp
public ThreadedCommentCollection ThreadedComments { get; }
```

### Exempel

```csharp

[C#]
ThreadedCommentCollection threadedComments = comment1.ThreadedComments;
for (int i = 0; i < threadedComments.Count; ++i)
{
    ThreadedComment tc = threadedComments[i];
    string note = tc.Notes;
}
```

### Se även

* class [ThreadedCommentCollection](../../threadedcommentcollection/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


