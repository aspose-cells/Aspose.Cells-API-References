---
title: "PageSetup.PrintTitleColumns"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PageSetup. تمثل الأعمدة التي تحتوي على الخلايا التي تُعاد على الجانب الأيسر من كل صفحة"
type: docs
url: /ar/net/aspose.cells/pagesetup/printtitlecolumns/
---
## PageSetup.PrintTitleColumns property

يمثل الأعمدة التي تحتوي على الخلايا التي ستُكرر على الجانب الأيسر من كل صفحة.

```csharp
public string PrintTitleColumns { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintTitleColumnsDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // الوصول إلى إعداد الصفحة
            PageSetup pageSetup = worksheet.PageSetup;
            
            // تعيين أعمدة عنوان الطباعة لتكرار العمود A في كل صفحة مطبوعة
            pageSetup.PrintTitleColumns = "$A:$A";
            
            // إضافة بعض البيانات إلى العمود A لتوضيح التأثير
            for (int i = 0; i < 50; i++)
            {
                worksheet.Cells[$"A{i + 1}"].PutValue($"Title Column - Row {i + 1}");
            }
            
            // احفظ المصنف
            workbook.Save("PrintTitleColumnsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


