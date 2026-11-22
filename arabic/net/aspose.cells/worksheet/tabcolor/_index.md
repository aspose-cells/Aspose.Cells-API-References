---
title: "Worksheet.TabColor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Worksheet. تمثل لون تبويب ورقة العمل"
type: docs
url: /ar/net/aspose.cells/worksheet/tabcolor/
---
## Worksheet.TabColor property

يمثل لون تبويب ورقة العمل.

```csharp
public Color TabColor { get; set; }
```

### ملاحظات

هذه الميزة مدعومة فقط في ExcelXP (Excel2002) والإصدارات الأحدث. إذا حفظت الملف بصيغة Excel97 أو Excel2000، سيتم حذفها.

### أمثلة

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyTabColorDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تعيين لون التبويب إلى الأحمر
            worksheet.TabColor = Color.Red;
            Console.WriteLine("Tab color set to: " + worksheet.TabColor);
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
            
            // مسح لون التبويب
            worksheet.TabColor = Color.Empty;
            Console.WriteLine("Tab color cleared: " + worksheet.TabColor.IsEmpty);
            
            // احفظ المصنف المعدل
            workbook.Save("output_modified.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


