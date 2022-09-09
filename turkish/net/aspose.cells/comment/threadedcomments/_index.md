---
title: ThreadedComments
second_title: Aspose.Cells for .NET API Referansı
description: Dizili yorumların listesini alır
type: docs
weight: 170
url: /tr/net/aspose.cells/comment/threadedcomments/
---
## Comment.ThreadedComments property

Dizili yorumların listesini alır;

```csharp
public ThreadedCommentCollection ThreadedComments { get; }
```

### Örnekler

```csharp

[C#]
ThreadedCommentCollection threadedComments = comment1.ThreadedComments;
for (int i = 0; i < threadedComments.Count; ++i)
{
    ThreadedComment tc = threadedComments[i];
    string note = tc.Notes;
}
```

### Ayrıca bakınız

* class [ThreadedCommentCollection](../../threadedcommentcollection)
* class [Comment](../../comment)
* ad alanı [Aspose.Cells](../../comment)
* toplantı [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->