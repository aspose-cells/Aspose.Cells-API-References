---
title: "Cell.Comment"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Cell. يحصل على التعليق لهذه الخلية"
type: docs
url: /ar/net/aspose.cells/cell/comment/
---
## Cell.Comment property

يحصل على التعليق الخاص بهذه الخلية.

```csharp
public Comment Comment { get; }
```

### ملاحظات

إذا لم يكن هناك تعليق يخص الخلية، تُرجع null.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellPropertyCommentDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة تعليق إلى الخلية A1
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Cell");

            // أضف تعليقًا إلى الخلية
            Comment comment = cell.Comment;
            if (comment == null)
            {
                // أنشئ تعليقًا جديدًا إذا لم يكن موجودًا
                int commentIndex = worksheet.Comments.Add("A1");
                comment = worksheet.Comments[commentIndex];
                comment.Author = "Author Name";
                comment.Note = "This is a sample comment";
            }

            try
            {
                // اعرض خصائص التعليق
                Console.WriteLine("Comment Author: " + comment.Author);
                Console.WriteLine("Comment Note: " + comment.Note);
                Console.WriteLine("Comment Row: " + comment.Row);
                Console.WriteLine("Comment Column: " + comment.Column);
                Console.WriteLine("Comment is Visible: " + comment.IsVisible);

                // عدّل بعض خصائص التعليق
                comment.Note = "Updated comment text";
                comment.IsVisible = true;

                // اعرض ملاحظة التعليق المحدثة
                Console.WriteLine("Updated Comment Note: " + comment.Note);

                // احفظ المصنف
                workbook.Save("CommentDemo.xlsx");
                Console.WriteLine("Comment has been demonstrated and saved to CommentDemo.xlsx");
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

* class [Comment](../../comment/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


