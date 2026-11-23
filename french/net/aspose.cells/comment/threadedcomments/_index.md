---
title: "Comment.ThreadedComments"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Comment. Obtient la liste des commentaires en fil"
type: docs
url: /fr/net/aspose.cells/comment/threadedcomments/
---
## Comment.ThreadedComments property

Obtient la liste des commentaires en fil de discussion ;

```csharp
public ThreadedCommentCollection ThreadedComments { get; }
```

### Exemples

```csharp

[C#]
ThreadedCommentCollection threadedComments = comment1.ThreadedComments;
for (int i = 0; i < threadedComments.Count; ++i)
{
    ThreadedComment tc = threadedComments[i];
    string note = tc.Notes;
}
```

### Voir aussi

* class [ThreadedCommentCollection](../../threadedcommentcollection/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


