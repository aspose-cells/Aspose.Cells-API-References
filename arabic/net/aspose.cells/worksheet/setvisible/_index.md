---
title: "Worksheet.SetVisible"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Worksheet. تحدد خيارات الرؤية"
type: docs
url: /ar/net/aspose.cells/worksheet/setvisible/
---
## Worksheet.SetVisible method

يضبط الخيارات المرئية.

```csharp
public void SetVisible(bool isVisible, bool ignoreError)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| isVisible | منطقي | ما إذا كانت ورقة العمل مرئية |
| ignoreError | منطقي | ما إذا كان يجب تجاهل الخطأ إذا لم يكن هذا الخيار صالحًا. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodSetVisibleWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // أضف بعض أوراق العمل
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // تعيين رؤية أوراق العمل
            // المعامل الأول: isVisible - false لإخفاء الورقة
            // المعامل الثاني: ignoreError - true لتجاهل الخطأ إذا تعذر إخفاء الورقة
            workbook.Worksheets["Sheet2"].SetVisible(false, true);
            workbook.Worksheets["Sheet3"].SetVisible(false, true);

            // احفظ المصنف
            workbook.Save("WorksheetVisibilityDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


