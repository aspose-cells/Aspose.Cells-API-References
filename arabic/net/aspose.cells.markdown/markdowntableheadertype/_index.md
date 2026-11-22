---
title: "التعداد MarkdownTableHeaderType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.Markdown.MarkdownTableHeaderType. يمثل نوع رأس الجدول في ملف markdown"
type: docs
url: /ar/net/aspose.cells.markdown/markdowntableheadertype/
---
## MarkdownTableHeaderType enumeration

يمثل نوع رأس الجدول في ملف markdown.

```csharp
public enum MarkdownTableHeaderType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| FirstRow | `0` | الصف الأول كرأس للجدول. |
| ColumnHeader | `1` | اسم العمود (مثل A,B,C...) كرأس للجدول. |
| Empty | `2` | صف رأس فارغ. |

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Markdown;

namespace AsposeCellsExamples
{
    public class MarkdownClassMarkdownTableHeaderTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية إلى الخلايا
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");

            // تعيين خيارات حفظ Markdown
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();
            saveOptions.TableHeaderType = MarkdownTableHeaderType.FirstRow;
            
            // حفظ كملف Markdown
            workbook.Save("output.md", saveOptions);
            
            // تحقق من المخرجات
            string text = File.ReadAllText("output.md");
            Console.WriteLine(text.Contains("---|") ? "Success" : "Failed");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Markdown](../../aspose.cells.markdown/)
* assembly [Aspose.Cells](../../)


