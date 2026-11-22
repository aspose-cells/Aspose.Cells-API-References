---
title: "Comment.ThreadedComments"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Comment. يحصل على قائمة التعليقات المتسلسلة"
type: docs
url: /ar/net/aspose.cells/comment/threadedcomments/
---
## Comment.ThreadedComments property

يحصل على قائمة التعليقات المتسلسلة؛

```csharp
public ThreadedCommentCollection ThreadedComments { get; }
```

### أمثلة

```csharp

[C#]
ThreadedCommentCollection threadedComments = comment1.ThreadedComments;
for (int i = 0; i < threadedComments.Count; ++i)
{
    ThreadedComment tc = threadedComments[i];
    string note = tc.Notes;
}
```

### انظر أيضًا

* class [ThreadedCommentCollection](../../threadedcommentcollection/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


