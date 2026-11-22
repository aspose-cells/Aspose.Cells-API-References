---
title: "Font.ScriptOffset"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Font. تحصل وتضبط إزاحة النص بوحدة النسبة المئوية"
type: docs
url: /ar/net/aspose.cells/font/scriptoffset/
---
## Font.ScriptOffset property

يحصل على ويضبط إزاحة النص، بوحدة النسبة المئوية

```csharp
public double ScriptOffset { get; set; }
```

### ملاحظات

فقط للأشكال والرسوم البيانية.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyScriptOffsetDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // الوصول إلى الخلية A1 وتعيين قيمتها
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("ScriptOffset Demo");

            // احصل على النمط وfont للخلية
            Style style = cell.GetStyle();
            Font font = style.Font;

            // اضبط ScriptOffset لتوضيح تأثير النص السفلي/العلوي
            font.ScriptOffset = 10; // Positive for superscript, negative for subscript
            font.IsSuperscript = true; // Enable superscript

            // تطبيق النمط المعدل مرة أخرى على الخلية
            cell.SetStyle(style);

            // احفظ المصنف
            workbook.Save("FontScriptOffsetDemo.xlsx");

            // تحقق من قيمة ScriptOffset
            Console.WriteLine("ScriptOffset value: " + font.ScriptOffset);
        }
    }
}
```

### انظر أيضًا

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


