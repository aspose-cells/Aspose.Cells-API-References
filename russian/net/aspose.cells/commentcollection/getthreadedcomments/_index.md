---
title: GetThreadedComments
second_title: Справочник по Aspose.Cells для .NET API
description: Получает связанные комментарии по индексу строки и столбца.
type: docs
weight: 50
url: /ru/net/aspose.cells/commentcollection/getthreadedcomments/
---
## GetThreadedComments(int, int) {#getthreadedcomments}

Получает связанные комментарии по индексу строки и столбца.

```csharp
public ThreadedCommentCollection GetThreadedComments(int row, int column)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| row | Int32 | Индекс строки. |
| column | Int32 | Индекс столбца. |

### Примеры

```csharp

[C#]
ThreadedCommentCollection threadedComments1 = comments.GetThreadedComments(1, 1);
for (int i = 0; i < threadedComments1.Count; ++i)
{
    ThreadedComment tc = threadedComments1[i];
    string note = tc.Notes;
}
```

### Смотрите также

* class [ThreadedCommentCollection](../../threadedcommentcollection)
* class [CommentCollection](../../commentcollection)
* пространство имен [Aspose.Cells](../../commentcollection)
* сборка [Aspose.Cells](../../../)

---

## GetThreadedComments(string) {#getthreadedcomments_1}

Получает цепочку комментариев по имени ячейки.

```csharp
public ThreadedCommentCollection GetThreadedComments(string cellName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| cellName | String | Имя ячейки. |

### Примеры

```csharp

[C#]
ThreadedCommentCollection threadedComments2 = comments.GetThreadedComments("B2");
for (int i = 0; i < threadedComments2.Count; ++i)
{
    ThreadedComment tc = threadedComments2[i];
    string note = tc.Notes;
}
```

### Смотрите также

* class [ThreadedCommentCollection](../../threadedcommentcollection)
* class [CommentCollection](../../commentcollection)
* пространство имен [Aspose.Cells](../../commentcollection)
* сборка [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->