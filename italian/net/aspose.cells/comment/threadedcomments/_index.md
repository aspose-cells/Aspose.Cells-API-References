---
title: "Comment.ThreadedComments"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Comment. Ottiene l'elenco dei commenti in thread"
type: docs
url: /it/net/aspose.cells/comment/threadedcomments/
---
## Comment.ThreadedComments property

Ottiene l'elenco dei commenti a thread;

```csharp
public ThreadedCommentCollection ThreadedComments { get; }
```

### Esempi

```csharp

[C#]
ThreadedCommentCollection threadedComments = comment1.ThreadedComments;
for (int i = 0; i < threadedComments.Count; ++i)
{
    ThreadedComment tc = threadedComments[i];
    string note = tc.Notes;
}
```

### Vedi anche

* class [ThreadedCommentCollection](../../threadedcommentcollection/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


