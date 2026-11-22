---
title: "ThreadedCommentCollection.Add"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ThreadedCommentCollection. تُضيف تعليقًا متسلسلًا"
type: docs
url: /ar/net/aspose.cells/threadedcommentcollection/add/
---
## ThreadedCommentCollection.Add method

يضيف تعليقًا متسلسلًا.

```csharp
public int Add(string text, ThreadedCommentAuthor author)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| نص | String | نص التعليق المتسلسل. |
| المؤلف | ThreadedCommentAuthor | مؤلف التعليق المتسلسل |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentCollectionMethodAddWithStringThreadedCommentDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات للسياق
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // إنشاء مؤلف تعليق متسلسل باستخدام ThreadedCommentAuthorCollection
                ThreadedCommentAuthorCollection authors = workbook.Worksheets.ThreadedCommentAuthors;
                int authorIndex = authors.Add("John Doe", "john.doe@example.com", "EXAMPLE_PROVIDER");
                ThreadedCommentAuthor author = authors[authorIndex];

                // الوصول إلى مجموعة التعليقات المتسلسلة لخلية
                Comment comment = worksheet.Comments[worksheet.Comments.Add("A1")];
                ThreadedCommentCollection threadedComments = comment.ThreadedComments;

                // استدعاء طريقة Add مع معلمات String و ThreadedCommentAuthor
                int commentIndex = threadedComments.Add("This is a threaded comment", author);

                // اعرض النتيجة
                Console.WriteLine($"Added threaded comment at index: {commentIndex}");
                Console.WriteLine($"Comment text: {threadedComments[commentIndex].Notes}");
                Console.WriteLine($"Author: {threadedComments[commentIndex].Author.Name}");

                // احفظ المصنف
                workbook.Save("ThreadedCommentAddDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [ThreadedCommentAuthor](../../threadedcommentauthor/)
* class [ThreadedCommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


