---
title: "Comment.ThreadedComments"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Comment özelliği. İş parçacıklı yorumların listesini alır"
type: docs
url: /tr/net/aspose.cells/comment/threadedcomments/
---
## Comment.ThreadedComments property

Zincirli yorumların listesini alır;

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

### Ayrıca Bakınız

* class [ThreadedCommentCollection](../../threadedcommentcollection/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


