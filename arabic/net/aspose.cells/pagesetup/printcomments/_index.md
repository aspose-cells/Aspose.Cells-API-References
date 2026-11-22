---
title: "PageSetup.PrintComments"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PageSetup. تمثل طريقة طباعة التعليقات مع الورقة"
type: docs
url: /ar/net/aspose.cells/pagesetup/printcomments/
---
## PageSetup.PrintComments property

يمثل طريقة طباعة التعليقات مع الورقة.

```csharp
public PrintCommentsType PrintComments { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintCommentsDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إضافة تعليق إلى الخلية A1
            int commentIndex = sheet.Comments.Add("A1");
            Comment comment = sheet.Comments[commentIndex];
            comment.Note = "This is a test comment";

            // تعيين خيارات طباعة التعليقات المختلفة وإظهار تأثيراتها
            sheet.PageSetup.PrintComments = PrintCommentsType.PrintInPlace;
            Console.WriteLine("PrintComments set to PrintInPlace");

            sheet.PageSetup.PrintComments = PrintCommentsType.PrintSheetEnd;
            Console.WriteLine("PrintComments set to PrintSheetEnd");

            sheet.PageSetup.PrintComments = PrintCommentsType.PrintNoComments;
            Console.WriteLine("PrintComments set to PrintNoComments");

            // احفظ المصنف لإظهار بقاء الإعدادات
            workbook.Save("PrintCommentsDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* enum [PrintCommentsType](../../printcommentstype/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


