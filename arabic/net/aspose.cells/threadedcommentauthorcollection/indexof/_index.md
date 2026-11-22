---
title: "ThreadedCommentAuthorCollection.IndexOf"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "ThreadedCommentAuthorCollection method. يحصل على فهرس كائن ThreadedCommentAuthor"
type: docs
url: /ar/net/aspose.cells/threadedcommentauthorcollection/indexof/
---
## ThreadedCommentAuthorCollection.IndexOf method

يحصل على فهرس كائن ThreadedCommentAuthor

```csharp
public int IndexOf(ThreadedCommentAuthor author)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| المؤلف | ThreadedCommentAuthor | كائن ThreadedCommentAuthor |

### قيمة الإرجاع

الفهرس في مجموعة ThreadedCommentAuthor

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentAuthorCollectionMethodIndexOfWithThreadedCommentAuthorDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // احصل على مجموعة مؤلفي التعليقات المتسلسلة
            ThreadedCommentAuthorCollection authors = workbook.Worksheets.ThreadedCommentAuthors;

            // أضف المؤلفين إلى المجموعة
            int johnIndex = authors.Add("John Doe", "john.doe", "provider1");
            int janeIndex = authors.Add("Jane Smith", "jane.smith", "provider2");

            // احصل على كائنات المؤلف
            ThreadedCommentAuthor johnAuthor = authors[johnIndex];
            ThreadedCommentAuthor janeAuthor = authors[janeIndex];

            try
            {
                // استدعِ طريقة IndexOf للعثور على موضع Jane Smith
                int foundIndex = authors.IndexOf(janeAuthor);
                
                // اعرض النتيجة
                Console.WriteLine($"Author '{janeAuthor.Name}' found at index: {foundIndex}");

                // تحقق من أن النتيجة تطابق الفهرس المتوقع
                if (foundIndex == janeIndex)
                {
                    Console.WriteLine("IndexOf result matches the expected index");
                }
                else
                {
                    Console.WriteLine("IndexOf result does not match the expected index");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing IndexOf method: {ex.Message}");
            }
            
            // احفظ المصنف
            workbook.Save("ThreadedCommentAuthorIndexOfDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ThreadedCommentAuthor](../../threadedcommentauthor/)
* class [ThreadedCommentAuthorCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


