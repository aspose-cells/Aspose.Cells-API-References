---
title: "ThreadedCommentAuthor.UserId"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ThreadedCommentAuthor. تحصل وتعيّن معرف المستخدم"
type: docs
url: /ar/net/aspose.cells/threadedcommentauthor/userid/
---
## ThreadedCommentAuthor.UserId property

يحصل على معرف المستخدم ويضبطه.

```csharp
public string UserId { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentAuthorPropertyUserIdDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // أضف مؤلف تعليق متسلسل بالاسم، userId، و providerId
                int authorIndex = workbook.Worksheets.ThreadedCommentAuthors.Add("John Doe", "JD123", "PROVIDER123");

                // احصل على كائن ThreadedCommentAuthor
                ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[authorIndex];

                // اعرض قيمة UserId (عملية قراءة)
                Console.WriteLine("Author UserId: " + author.UserId);

                // أظهر تعيين UserId جديد (عملية كتابة)
                author.UserId = "NEW_USER_ID";
                Console.WriteLine("Updated UserId: " + author.UserId);

                // أنشئ تعليقًا متسلسلًا باستخدام المؤلف
                worksheet.Comments.AddThreadedComment("A1", "This is a sample comment", author);

                // احفظ المصنف
                workbook.Save("UserIdDemo.xlsx");

                Console.WriteLine("UserId property demonstration completed successfully.");
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

* class [ThreadedCommentAuthor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


