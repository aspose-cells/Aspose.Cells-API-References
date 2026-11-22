---
title: "TxtSaveOptions.Separator"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TxtSaveOptions. يحصل ويضبط فاصل الحرف لملف النص"
type: docs
url: /ar/net/aspose.cells/txtsaveoptions/separator/
---
## TxtSaveOptions.Separator property

يحصل على ويضبط char Delimiter لملف النص.

```csharp
public char Separator { get; set; }
```

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertySeparatorDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل تجريبي مع بيانات اختبار
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // قم بتكوين خيارات حفظ TXT باستخدام الفاصل الفاصلة
            TxtSaveOptions txtSaveOptions = new TxtSaveOptions();
            txtSaveOptions.Separator = ',';
            txtSaveOptions.Encoding = System.Text.Encoding.UTF8;

            // احفظ المصنف كـ CSV باستخدام الفاصل الفاصلة
            string outputPath = "output.csv";
            workbook.Save(outputPath, txtSaveOptions);

            // اعرض محتوى الملف المحفوظ
            Console.WriteLine("File saved with comma separator:");
            Console.WriteLine(File.ReadAllText(outputPath));
        }
    }
}
```

### انظر أيضًا

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


