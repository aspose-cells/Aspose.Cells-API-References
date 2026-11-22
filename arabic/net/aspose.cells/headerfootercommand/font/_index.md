---
title: "HeaderFooterCommand.Font"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HeaderFooterCommand. يحصل على الخط لقيمة الأمر"
type: docs
url: /ar/net/aspose.cells/headerfootercommand/font/
---
## HeaderFooterCommand.Font property

يسترجع الخط لقيمة الأمر.

```csharp
public Font Font { get; }
```

### ملاحظات

غير مفيد لـ HeaderFooterCommandType.Picture.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HeaderFooterCommandPropertyFontDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // الوصول إلى إعداد الصفحة للرأس/التذييل
            PageSetup pageSetup = worksheet.PageSetup;

            // تعيين رأس بنص سيحتوي على HeaderFooterCommand
            pageSetup.SetHeader(0, "&\"Arial\"&12&BThis is a header");

            // الحصول على سكريبت الرأس
            string headerScript = pageSetup.GetHeader(0);

            // احصل على أوامر الرأس
            HeaderFooterCommand[] commands = pageSetup.GetCommands(headerScript);

            // البحث عن أمر النص (مع افتراض أنه الأول)
            if (commands.Length > 0 && commands[0].Type == HeaderFooterCommandType.Text)
            {
                HeaderFooterCommand textCommand = commands[0];
                
                // الوصول إلى خاصية Font (للقراءة فقط)
                Font font = textCommand.Font;
                
                // عرض خصائص الخط الحالية
                Console.WriteLine("Current Font:");
                Console.WriteLine($"Name: {font.Name}");
                Console.WriteLine($"Size: {font.Size}");
                Console.WriteLine($"Bold: {font.IsBold}");
                Console.WriteLine($"Color: {font.Color}");

                // نظرًا لأن Font للقراءة فقط، لا يمكننا تعيين كائن Font جديد،
                // ولكن يمكننا تعديل خصائص الخط الحالية
                font.Name = "Times New Roman";
                font.Size = 14;
                font.IsBold = false;
                font.Color = System.Drawing.Color.Blue;

                // احفظ المصنف لرؤية التغييرات
                workbook.Save("HeaderFooterFontDemo.xlsx");

                Console.WriteLine("\nModified Font:");
                Console.WriteLine($"Name: {font.Name}");
                Console.WriteLine($"Size: {font.Size}");
                Console.WriteLine($"Bold: {font.IsBold}");
                Console.WriteLine($"Color: {font.Color}");
            }
        }
    }
}
```

### انظر أيضًا

* class [Font](../../font/)
* class [HeaderFooterCommand](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


