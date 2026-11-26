---
title: "CommentCollection.GetThreadedComments"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод CommentCollection. Получает ветвленные комментарии по индексу строки и столбца"
type: docs
url: /ru/net/aspose.cells/commentcollection/getthreadedcomments/
---
## GetThreadedComments(int, int) {#getthreadedcomments}

Получает ветвящиеся комментарии по индексу строки и столбца.

```csharp
public ThreadedCommentCollection GetThreadedComments(int row, int column)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | Int32 | Индекс строки. |
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

### См. также

* class [ThreadedCommentCollection](../../threadedcommentcollection/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetThreadedComments(string) {#getthreadedcomments_1}

Получает ветвящиеся комментарии по имени ячейки.

```csharp
public ThreadedCommentCollection GetThreadedComments(string cellName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| cellName | String | Имя ячейки. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentCollectionMethodGetThreadedCommentsWithStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить автора ветвленного комментария и получить автора по индексу
            int authorIndex = workbook.Worksheets.ThreadedCommentAuthors.Add("John Doe", "JD", "1");
            ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[authorIndex];

            // Добавить ветвленный комментарий в ячейку B2
            worksheet.Comments.AddThreadedComment("B2", "Initial comment", author);

            // Получить все ветвленные комментарии для ячейки B2
            ThreadedCommentCollection threadedComments = worksheet.Comments.GetThreadedComments("B2");

            // Отобразить ветвленные комментарии
            foreach (ThreadedComment comment in threadedComments)
            {
                Console.WriteLine($"Comment by {comment.Author.Name}: {comment.Notes}");
            }
        }
    }
}
```

### См. также

* class [ThreadedCommentCollection](../../threadedcommentcollection/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


