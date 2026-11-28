---
title: "CommentCollection.GetThreadedComments"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CommentCollection yöntemi. Satır ve sütun indeksine göre zincirlenmiş yorumları alır"
type: docs
url: /tr/net/aspose.cells/commentcollection/getthreadedcomments/
---
## GetThreadedComments(int, int) {#getthreadedcomments}

Satır ve sütun indeksine göre iş parçacıklı yorumları alır.

```csharp
public ThreadedCommentCollection GetThreadedComments(int row, int column)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | Int32 | Satır indeksi. |
| sütun | Int32 | Sütun indeksi. |

### Örnekler

```csharp

[C#]
ThreadedCommentCollection threadedComments1 = comments.GetThreadedComments(1, 1);
for (int i = 0; i < threadedComments1.Count; ++i)
{
    ThreadedComment tc = threadedComments1[i];
    string note = tc.Notes;
}
```

### Ayrıca Bakınız

* class [ThreadedCommentCollection](../../threadedcommentcollection/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetThreadedComments(string) {#getthreadedcomments_1}

Hücre adıyla iş parçacıklı yorumları alır.

```csharp
public ThreadedCommentCollection GetThreadedComments(string cellName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cellName | String | Hücrenin adı. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentCollectionMethodGetThreadedCommentsWithStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Zincirlenmiş yorum yazarını ekle ve yazarını indeksle al
            int authorIndex = workbook.Worksheets.ThreadedCommentAuthors.Add("John Doe", "JD", "1");
            ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[authorIndex];

            // B2 hücresine zincirlenmiş bir yorum ekle
            worksheet.Comments.AddThreadedComment("B2", "Initial comment", author);

            // B2 hücresi için tüm zincirli yorumları alın
            ThreadedCommentCollection threadedComments = worksheet.Comments.GetThreadedComments("B2");

            // Zincirli yorumları görüntüle
            foreach (ThreadedComment comment in threadedComments)
            {
                Console.WriteLine($"Comment by {comment.Author.Name}: {comment.Notes}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [ThreadedCommentCollection](../../threadedcommentcollection/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


