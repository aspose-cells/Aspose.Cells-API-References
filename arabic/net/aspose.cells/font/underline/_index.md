---
title: "Font.Underline"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية الخط. تحصل أو تعين نوع تسطير الخط"
type: docs
url: /ar/net/aspose.cells/font/underline/
---
## Font.Underline property

يحصل على أو يضبط نوع تسطير الخط.

```csharp
public FontUnderlineType Underline { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyUnderlineDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // الوصول إلى الخلية وتعيين نمط التسطير
            Cell cell = sheet.Cells["A1"];
            cell.PutValue("Sample Underlined Text");
            
            // احصل على النمط وعدّل خصائص الخط
            Style style = cell.GetStyle();
            style.Font.Underline = FontUnderlineType.Single;
            cell.SetStyle(style);

            // احفظ المصنف
            workbook.Save("FontUnderlineDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [FontUnderlineType](../../fontunderlinetype/)
* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


