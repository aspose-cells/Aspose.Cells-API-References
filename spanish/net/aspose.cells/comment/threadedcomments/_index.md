---
title: "Comment.ThreadedComments"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Comment. Obtiene la lista de comentarios en hilo"
type: docs
url: /es/net/aspose.cells/comment/threadedcomments/
---
## Comment.ThreadedComments property

Obtiene la lista de comentarios en hilo;

```csharp
public ThreadedCommentCollection ThreadedComments { get; }
```

### Ejemplos

```csharp

[C#]
ThreadedCommentCollection threadedComments = comment1.ThreadedComments;
for (int i = 0; i < threadedComments.Count; ++i)
{
    ThreadedComment tc = threadedComments[i];
    string note = tc.Notes;
}
```

### Ver también

* class [ThreadedCommentCollection](../../threadedcommentcollection/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


