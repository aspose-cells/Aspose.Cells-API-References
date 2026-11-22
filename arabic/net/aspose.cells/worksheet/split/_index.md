---
title: "Worksheet.Split"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Worksheet. تقسم النافذة"
type: docs
url: /ar/net/aspose.cells/worksheet/split/
---
## Worksheet.Split method

يقسم النافذة.

```csharp
public void Split()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodSplitDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة لتوضيح التقسيم
            worksheet.Cells["A1"].PutValue("Header");
            for (int i = 1; i <= 50; i++)
            {
                worksheet.Cells["A" + (i + 1)].PutValue("Data " + i);
            }
            
            // تقسيم worksheet (لا حاجة إلى معلمات)
            worksheet.Split();
            
            // احفظ المصنف
            workbook.Save("WorksheetSplitDemo.xml", SaveFormat.SpreadsheetML);
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


