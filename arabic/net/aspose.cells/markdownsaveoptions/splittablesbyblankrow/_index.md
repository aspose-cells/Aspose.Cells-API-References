---
title: "MarkdownSaveOptions.SplitTablesByBlankRow"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية MarkdownSaveOptions. تشير إلى ما إذا كان يجب اعتبار الصفوف الفارغة في ورقة العمل كفواصل للجداول عند التصدير إلى Markdown. القيمة الافتراضية هي false"
type: docs
url: /ar/net/aspose.cells/markdownsaveoptions/splittablesbyblankrow/
---
## MarkdownSaveOptions.SplitTablesByBlankRow property

يحدد ما إذا كان يجب اعتبار الصفوف الفارغة في ورقة العمل كفواصل جدول عند التصدير إلى Markdown. القيمة الافتراضية هي false.

```csharp
public bool SplitTablesByBlankRow { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownSaveOptionsPropertySplitTablesByBlankRowDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات عينة مع صفوف فارغة لتوضيح تقسيم الجداول
            worksheet.Cells["A1"].Value = "Table 1 Header";
            worksheet.Cells["B1"].Value = "Value 1";
            worksheet.Cells["A2"].Value = "Data 1";
            worksheet.Cells["B2"].Value = "Data 2";

            // أضف صفًا فارغًا (الصف 3)
            worksheet.Cells["A4"].Value = "Table 2 Header";
            worksheet.Cells["B4"].Value = "Value 2";
            worksheet.Cells["A5"].Value = "Data 3";
            worksheet.Cells["B5"].Value = "Data 4";

            // إنشاء مثيل MarkdownSaveOptions
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

            try
            {
                // اعرض القيمة الافتراضية لـ SplitTablesByBlankRow
                Console.WriteLine("Default SplitTablesByBlankRow value: " +
                    saveOptions.SplitTablesByBlankRow);

                // عيّن SplitTablesByBlankRow إلى true لتقسيم الجداول حسب الصفوف الفارغة
                saveOptions.SplitTablesByBlankRow = true;

                // عرض القيمة المحدثة
                Console.WriteLine("Updated SplitTablesByBlankRow value: " +
                    saveOptions.SplitTablesByBlankRow);

                // احفظ المصنف كملف markdown مع تمكين تقسيم الجداول
                workbook.Save("SplitTablesByBlankRowDemo.md", saveOptions);
                Console.WriteLine("Markdown file saved with table splitting by blank rows enabled.");
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


