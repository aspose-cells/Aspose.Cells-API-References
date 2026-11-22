---
title: "Workbook.DefaultStyle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Workbook. تحصل أو تعين كائن Style الافتراضي للدفتر"
type: docs
url: /ar/net/aspose.cells/workbook/defaultstyle/
---
## Workbook.DefaultStyle property

تحصل أو تعين كائن [`Style`](../../style/) الافتراضي للدفتر.

```csharp
public Style DefaultStyle { get; set; }
```

### ملاحظات

خاصية DefaultStyle مفيدة لتطبيق Style على كامل Workbook.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyDefaultStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // احصل على النمط الافتراضي وعدل الخط الخاص به
            Style defaultStyle = workbook.DefaultStyle;
            defaultStyle.Font.Name = "Tahoma";
            defaultStyle.Font.Size = 12;
            
            // تطبيق النمط المعدل مرة أخرى كافتراضي
            workbook.DefaultStyle = defaultStyle;
            
            // إنشاء ورقة عمل وإضافة بعض النص باستخدام النمط الافتراضي
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("This text uses the default Tahoma font");
            
            // احفظ المصنف
            workbook.Save("DefaultStyleDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Style](../../style/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


