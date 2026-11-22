---
title: "Font.IsSuperscript"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية الخط. تحصل أو تعين قيمة تشير إلى ما إذا كان الخط مرفوع"
type: docs
url: /ar/net/aspose.cells/font/issuperscript/
---
## Font.IsSuperscript property

يحصل على أو يضبط قيمة تشير إلى ما إذا كان الخط مرتفعًا.

```csharp
public bool IsSuperscript { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyIsSuperscriptDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف نصًا إلى الخلية A1
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Normal Text Superscript Text");
            
            // تنسيق جزء من النص كمرتفع
            FontSetting setting = cell.Characters(12, 11);
            setting.Font.IsSuperscript = true;
            
            // احفظ المصنف
            workbook.Save("FontIsSuperscriptDemo.xlsx");
            
            // تحقق من إعداد النص العلوي
            Console.WriteLine("IsSuperscript property: " + setting.Font.IsSuperscript);
        }
    }
}
```

### انظر أيضًا

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


