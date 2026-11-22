---
title: "ThreadedCommentAuthor.ProviderId"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ThreadedCommentAuthor. تحصل على معرف الموفر"
type: docs
url: /ar/net/aspose.cells/threadedcommentauthor/providerid/
---
## ThreadedCommentAuthor.ProviderId property

يحصل على معرف الموفر.

```csharp
public string ProviderId { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentAuthorPropertyProviderIdDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            try
            {
                // أضف مؤلف تعليق متسلسل واحصل على فهرسه
                int authorIndex = workbook.Worksheets.ThreadedCommentAuthors.Add("John Doe", "JD123", "PROVIDER123");
                
                // احصل على كائن ThreadedCommentAuthor
                ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[authorIndex];
                
                // اعرض قيمة ProviderId (عملية قراءة)
                Console.WriteLine("Author ProviderId: " + author.ProviderId);
                
                // أنشئ تعليقًا متسلسلًا باستخدام المؤلف
                worksheet.Comments.AddThreadedComment("A1", "This is a sample comment", author);
                
                // احفظ المصنف
                workbook.Save("ThreadedCommentAuthorDemo.xlsx");
                
                Console.WriteLine("Demo completed successfully.");
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


