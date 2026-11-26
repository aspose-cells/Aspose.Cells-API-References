---
title: "Comment.ThreadedComments"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Comment. Возвращает список вложенных комментариев"
type: docs
url: /ru/net/aspose.cells/comment/threadedcomments/
---
## Comment.ThreadedComments property

Получает список ветвистых комментариев;

```csharp
public ThreadedCommentCollection ThreadedComments { get; }
```

### Примеры

```csharp

[C#]
ThreadedCommentCollection threadedComments = comment1.ThreadedComments;
for (int i = 0; i < threadedComments.Count; ++i)
{
    ThreadedComment tc = threadedComments[i];
    string note = tc.Notes;
}
```

### См. также

* class [ThreadedCommentCollection](../../threadedcommentcollection/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


