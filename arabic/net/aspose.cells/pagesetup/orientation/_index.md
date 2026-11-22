---
title: "PageSetup.Orientation"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PageSetup. تمثل اتجاه طباعة الصفحة"
type: docs
url: /ar/net/aspose.cells/pagesetup/orientation/
---
## PageSetup.Orientation property

يمثل اتجاه طباعة الصفحة.

```csharp
public PageOrientationType Orientation { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyOrientationDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تعيين اتجاه الصفحة إلى Landscape
            worksheet.PageSetup.Orientation = PageOrientationType.Landscape;
            
            // أضف بعض البيانات النموذجية لتوضيح التأثير
            worksheet.Cells["A1"].PutValue("Landscape Orientation Demo");
            for (int i = 1; i <= 10; i++)
            {
                worksheet.Cells[$"A{i}"].PutValue($"Data Row {i}");
            }
            
            // احفظ المصنف
            workbook.Save("PageOrientationDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* enum [PageOrientationType](../../pageorientationtype/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


