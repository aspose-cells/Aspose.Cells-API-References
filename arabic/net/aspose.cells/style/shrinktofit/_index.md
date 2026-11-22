---
title: "Style.ShrinkToFit"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Style. تمثل ما إذا كان النص يتقلص تلقائيًا ليتناسب مع عرض العمود المتاح"
type: docs
url: /ar/net/aspose.cells/style/shrinktofit/
---
## Style.ShrinkToFit property

يمثل ما إذا كان النص يتقلص تلقائيًا ليتناسب مع عرض العمود المتاح.

```csharp
public bool ShrinkToFit { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyShrinkToFitDemo
    {
        public static void Run()
        {
            // إنشاء كائن دفتر عمل
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // الوصول إلى مجموعة الخلايا
            Cells cells = worksheet.Cells;
            
            // ضع بعض النص في الخلية A1 يكون أطول من عرض العمود
            cells["A1"].PutValue("This is a long text that needs shrinking to fit");
            
            // عيّن عرض العمود ليكون أصغر من طول النص
            cells.SetColumnWidth(0, 10);
            
            // احصل على نمط الخلية A1
            Style style = cells["A1"].GetStyle();
            
            // عيّن ShrinkToFit إلى true
            style.ShrinkToFit = true;
            
            // تطبيق النمط على الخلية A1
            cells["A1"].SetStyle(style);
            
            // احفظ المصنف
            workbook.Save("ShrinkToFitDemo.xlsx");
            
            Console.WriteLine("ShrinkToFit demo completed successfully.");
        }
    }
}
```

### انظر أيضًا

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


