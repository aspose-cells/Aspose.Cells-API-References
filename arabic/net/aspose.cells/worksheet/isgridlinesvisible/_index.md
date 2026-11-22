---
title: "Worksheet.IsGridlinesVisible"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Worksheet. تحصل أو تعين قيمة تشير إلى ما إذا كانت خطوط الشبكة مرئية. القيمة الافتراضية هي true"
type: docs
url: /ar/net/aspose.cells/worksheet/isgridlinesvisible/
---
## Worksheet.IsGridlinesVisible property

يحصل على أو يضبط قيمة تشير إلى ما إذا كانت خطوط الشبكة مرئية. القيمة الافتراضية هي true.

```csharp
public bool IsGridlinesVisible { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsGridlinesVisibleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تعيين رؤية خطوط الشبكة إلى true
            worksheet.IsGridlinesVisible = true;
            
            // إضافة بعض البيانات التجريبية لرؤية خطوط الشبكة
            worksheet.Cells["A1"].PutValue("Gridlines Visible Example");
            worksheet.Cells["A2"].PutValue("This worksheet shows gridlines");
            
            // ضبط الأعمدة تلقائيًا لتحسين الرؤية
            worksheet.AutoFitColumns();
            
            // احفظ المصنف
            workbook.Save("GridlinesVisibleDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


