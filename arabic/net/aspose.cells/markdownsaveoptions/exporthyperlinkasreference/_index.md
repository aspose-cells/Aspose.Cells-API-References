---
title: "MarkdownSaveOptions.ExportHyperlinkAsReference"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية MarkdownSaveOptions. تشير إلى ما إذا كان يجب تصدير الارتباط التشعبي باستخدام تعريفات مرجعية بدلاً من التنسيق المضمن. القيمة الافتراضية هي false"
type: docs
url: /ar/net/aspose.cells/markdownsaveoptions/exporthyperlinkasreference/
---
## MarkdownSaveOptions.ExportHyperlinkAsReference property

يشير إلى ما إذا كان يجب تصدير الارتباط التشعبي باستخدام تعريفات المرجع بدلاً من الصيغة المضمنة. القيمة الافتراضية هي false.

```csharp
public bool ExportHyperlinkAsReference { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownSaveOptionsPropertyExportHyperlinkAsReferenceDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا جديدًا واحصل على ورقة العمل الأولى
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // ضع نصًا عينيًا في خلية
            sheet.Cells["A1"].PutValue("Visit Aspose");

            // أضف ارتباطًا تشعبيًا إلى الخلية (A1)
            // المعلمات: firstRow, firstColumn, totalRows, totalColumns, hyperlink
            sheet.Hyperlinks.Add(0, 0, 1, 1, "https://www.aspose.com");

            // تهيئة خيارات حفظ Markdown
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

            try
            {
                // الوصول مباشرة إلى خاصية ExportHyperlinkAsReference (للقراءة فقط في هذا العرض التوضيحي)
                Console.WriteLine("ExportHyperlinkAsReference value: " + saveOptions.ExportHyperlinkAsReference);

                // احفظ المصنف كملف markdown؛ الخاصية (إذا كانت true) ستؤثر على طريقة تصدير الارتباطات التشعبية
                workbook.Save("ExportHyperlinkAsReferenceDemo.md", saveOptions);
                Console.WriteLine("Workbook saved as markdown.");
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

* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


